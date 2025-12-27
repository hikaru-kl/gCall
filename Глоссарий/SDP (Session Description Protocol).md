[**SDP**]([Session Description Protocol — Википедия](https://ru.wikipedia.org/wiki/Session_Description_Protocol)) — это текстовое описание параметров мультимедийной сессии.

## Что описывает SDP

SDP отвечает на вопрос:

> «Какие медиа мы будем передавать и как?»

В SDP содержится:

- типы медиа (audio / video)
    
- кодеки (Opus, VP8 и т.д.)
    
- IP и порты
    
- направления потоков (sendrecv)
    
- параметры шифрования
    
- ICE информация
    

## Формат

SDP — это **plain text**, пример:

```
m=audio 9 UDP/TLS/RTP/SAVPF 111
a=rtpmap:111 opus/48000/2
a=sendrecv
```

## Роль в WebRTC

- SDP **обмениваются через signaling**
    
- используется для согласования параметров
    
- существует offer / answer модель
    

## Важное

- SDP **не передаёт медиа**
    
- это только **описание будущего соединения**