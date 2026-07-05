# Telegram avansat
- Butoane inline: in sendMessage adaugi reply_markup:{inline_keyboard:[[{text:'Aproba',callback_data:'ok'},{text:'Nu',callback_data:'no'}]]}.
- Primesti update.callback_query cu .data si .from.id; raspunzi cu answerCallbackQuery ca sa dispara loading-ul.
- Trimite poza: sendPhoto {chat_id,photo:url_sau_file_id,caption}. Fisier: sendDocument.
- Meniu comenzi: setMyCommands. Grup: verifica message.chat.type. Editare mesaj: editMessageText.
