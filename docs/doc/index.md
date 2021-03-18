# Документация Node.js

**Node.js** - это программная платформа, которая предоставляет среду для выполнения кода JavaScript на стороне сервера.

!!! note ""

    Node.js не является языком программирования, код пишется на JavaScript.

В отличие от PHP, который работает под управлением "стороннего" веб-сервера, например, Apache или IIS, Node.js сама является веб-сервером. Но часто она работает в связке с Nginx в качестве основного сервера. Использование Nginx совсем не обязательно, но оправдано для кэширования данных запроса, отдачи статических файлов или разделения доменов в пределах одного сервера (reverse proxy).

В основе Node.js лежит разработанный Google движок V8, который используется в браузере Chrome и отвечает за компиляцию кода JavaScript во внутренний код машины. На этом причастность Google заканчивается. На самом деле платформу создал Райан Даль, а спонсированием ее разработки занимается компания Joyent.

Node.js относится к событийно-ориентированным системам и использует модель выполнения операций ввода-вывода (I/O) таким образом, что основной процесс никогда не блокируется, за исключением редких случаев. А отсутствие единого блокируемого потока выполнения позволяет создавать эффективные, высокопроизводительные и легко масштабируемые серверные приложения.

!!! note ""

    Node.js это однопоточная событийно-ориентированная система.

!!! note ""

    Если в среде работы Node.js приложения большего одного ядра, то они могут быть использованы для запуска дочерних процессов, которые могут распределить на себя нагрузку основного процесса. Это называется [кластеризацией](cluster.md).

На данный момент Node.js не является частью ни одной из существующих операционных систем и поэтому требует отдельной [установки](https://nodejs.org/en/download/).