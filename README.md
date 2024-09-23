from flask import Flask, jsonify
import random
from responses import magic_8_ball_responses

app = Flask(__name__)

#AppRoutePythonFlask
@app.route('/api/magic8ball', methods=['GET'])
def get_magic_8_ball_response():
    # Pick a random response from the list
    response = random.choice(magic_8_ball_responses)
    return jsonify({'response': response})

if __name__ == '__main__':
    app.run(debug=True)

from flask import Flask, jsonify
import random
from responses import magic_8_ball_responses

app = Flask(__name__)

#RandomChoice
@app.route('/api/magic8ball', methods=['GET'])
def get_magic_8_ball_response():
    # Pick a random response from the list
    response = random.choice(magic_8_ball_responses)
    return jsonify({'response': response})

if __name__ == '__main__':
    app.run(debug=True)
