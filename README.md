# EventBridge_Dev

💡 Explicação Simples:
O EventBridge é um serviço de event-driven, ou seja, funciona baseado em eventos. Quando alguma coisa acontece em um serviço (tipo subir um arquivo no S3, criar uma instância EC2, ou uma notificação de um app externo tipo Zendesk, Shopify, Auth0…), ele dispara um evento. Esse evento aciona uma regra que executa uma ação, como ligar uma Lambda, uma Step Function, uma fila do SQS, SNS, etc.

🔥 Na prática é tipo:
“Opa! Subiu um arquivo no S3” → EventBridge percebe → “Beleza, vou chamar a Lambda pra processar isso.”

“Alguém cadastrou um usuário no sistema” → EventBridge percebe → “Bora acionar um SNS pra avisar o time.”

🧠 O que ele faz:
Conecta serviços da AWS entre si (sem precisar você ficar codando integração maluca);

Conecta aplicações externas (SaaS) direto na AWS;

Roteia eventos baseados em regras (tipo, se evento for X, faz Y);

É serverless, então você não se preocupa em subir servidor pra isso.

⚡ Diferença pro SNS e SQS:
SNS e SQS são mensagerias, mas o EventBridge tem muito mais poder pra criar regras inteligentes e filtrar eventos super específicos.

SNS é tipo "manda mensagem pra geral", EventBridge é "manda mensagem pra quem se encaixa nessa regra aqui ó 👀".

🚀 Quando usar EventBridge?
Quando quiser automação baseada em eventos;

Quando precisa conectar vários serviços de forma desacoplada;

Quando quer integração com sistemas externos direto na AWS.

🎯 Resumo de 1 linha:
O EventBridge é o serviço que escuta eventos e dispara ações na AWS, de forma inteligente, escalável e sem servidor.


