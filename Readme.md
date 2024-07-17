Link para o Codificador no Vercel: https://codedecode1.vercel.app/

Minha maior dificuldade foi com o código javaScript, colocarei a explicação das areas que tive dificuldade para entender

Explicando o JavaScript

Como funciona:
Eventos de Clique:

Quando você clica no botão com o ID encodeButton, a função encodeText é chamada.
Quando você clica no botão com o ID decodeButton, a função decodeText é chamada.

Função encodeText:

Pega o texto do campo de entrada com o ID inputText.
Se o campo estiver vazio, chama a função displayNoMessage.
Se não estiver vazio, codifica o texto em Base64 usando btoa e exibe o resultado no campo outputText.
Se o texto for codificado com sucesso, chama a função hideNoMessage para garantir que a mensagem de erro (se existir) seja escondida.

Função decodeText:

Pega o texto do campo de entrada com o ID inputText.
Se o campo estiver vazio, chama a função displayNoMessage.
Se não estiver vazio, tenta decodificar o texto de Base64 usando atob.
Se a decodificação for bem-sucedida, exibe o texto decodificado no campo outputText.
Se a decodificação falhar (por exemplo, se o texto não estiver no formato Base64), mostra um alerta com a mensagem "Texto inválido para decodificação!".

Funções displayNoMessage e hideNoMessage:

displayNoMessage mostra uma mensagem de erro e esconde o campo de saída (outputText).
hideNoMessage esconde a mensagem de erro e mostra o campo de saída (outputText).
