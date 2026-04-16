# Lab: GitHub Actions - Variáveis

## Perguntas de Reflexão

### 1. Por que a Secret aparece no log como `***` e a variável aparece normalmente?

**Resposta:** Pois é um valor sensível e possui uma máscara ocultando seu valor, mesmo que seja exibido com `echo`.

### 2. O Job 2 consegue ler a variável BUILD_VERSION criada no Job 1? Por que?

**Resposta:** Não, pois cada job roda em uma máquina separada e variáveis de ambiente não são compartilhadas entre jobs.