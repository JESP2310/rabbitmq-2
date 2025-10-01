RabbitMQ Task Queue - Python

Este projeto contém dois scripts Python que demonstram o uso de fila de tarefas com RabbitMQ:

Producer (send_task.py): envia mensagens para a fila task_queue, que são persistentes e podem incluir texto passado como argumento.

Consumer (worker.py): consome mensagens da fila, processa cada tarefa simulando tempo de execução e confirma manualmente (basic_ack) para garantir que mensagens não sejam perdidas.

Funcionalidades principais:

Mensagens persistentes na fila (durable=True).

Distribuição de tarefas entre múltiplos workers.

Processamento seguro com confirmação manual.

Simulação de tarefas demoradas baseada no conteúdo da mensagem.

Uso esperado:

Executar RabbitMQ localmente.

Rodar o producer para enviar mensagens e o consumer para processá-las.

No Management UI, ver a fila com mensagens Ready ou Unacknowledged até serem confirmadas.

Esses scripts mostram o funcionamento básico de Producer-Consumer e como implementar uma task queue confiável com Python e RabbitMQ.
