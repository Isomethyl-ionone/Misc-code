class CaesarCipher {
  constructor(shift){
        this.encode = function(encoded) {
          var alphabet = ["a", "b", "c", "d", "e", "f", "g", "h", "i", "j", "k", "l", "m", "n", "o", "p", "q", "r", "s", "t", "u", "v", "w", "x", "y", "z"];
          var encodedMessage = encoded.toLowerCase();
          var decodedMessage = '';
            for (var i = 0; i < encoded.length; i++) {
              if (alphabet.indexOf(encodedMessage.charAt(i)) === -1) {
                decodedMessage += encodedMessage.charAt(i);
                }
              else if(alphabet.indexOf(encodedMessage.charAt(i)) + shift < alphabet.length) {
                    decodedMessage += (alphabet[alphabet.indexOf(encodedMessage.charAt(i)) + shift]);
                    }
                    else {
                      var overflow = alphabet.indexOf(encodedMessage.charAt(i)) + shift - alphabet.length;
                      decodedMessage += (alphabet[overflow]);
                      }    
               }  
          decodedMessage = decodedMessage.toUpperCase();
          return decodedMessage
          }; 

      this.decode = function(decoded) {
        var alphabet = ["a", "b", "c", "d", "e", "f", "g", "h", "i", "j", "k", "l", "m", "n", "o", "p", "q", "r", "s", "t", "u", "v", "w", "x", "y", "z"];
        var Message = decoded.toLowerCase();
        var encodedMessage = '';
          for (var i = 0; i < Message.length; i++) {
            if (alphabet.indexOf(Message.charAt(i)) === -1) {
              encodedMessage += Message.charAt(i);
              }
            else if (alphabet.indexOf(Message.charAt(i)) - shift >= 0) {
                  encodedMessage += (alphabet[alphabet.indexOf(Message.charAt(i)) - shift]);
                  }
                  else {
                    var overflow = alphabet.indexOf(Message.charAt(i)) + alphabet.length - shift;
                    encodedMessage += (alphabet[overflow]);
                    }
            }   
        encodedMessage = encodedMessage.toUpperCase();  
        return encodedMessage
        };
  }
}
