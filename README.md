# arquitetura

Visão Executiva
O HealthSync resolve a fragmentação do cuidado remoto ao unificar teleconsultas, dados de dispositivos IoT (wearables) e suporte à decisão clínica via IA em uma única plataforma digital. O problema central enfrentado pelo mercado de digital health é a falta de monitoramento contínuo e personalizado, que atrasa diagnósticos críticos e sobrecarrega os sistemas de saúde tradicionais.

Estado atual — Fase 3
Na Fase 3, o projeto evolui de um Monólito Modular (Fases 1–3) para uma arquitetura orientada a microsserviços implantada em nuvem (AWS), preservando os princípios de Hexagonal Architecture e Clean Architecture no núcleo de cada serviço. Os principais avanços desta fase são:

Implantação em AWS com modelo híbrido PaaS + Serverless;
API Gateway como ponto único de entrada com autenticação JWT/OAuth2;
Circuit Breaker (Resilience4j) protegendo integrações críticas com HIS e APIs de IA externas;
Comunicação assíncrona via Amazon SQS/SNS para ingestão de dados IoT e notificações;
Observabilidade completa com CloudWatch + AWS X-Ray.
