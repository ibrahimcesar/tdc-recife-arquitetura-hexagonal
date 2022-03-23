<div align="center">

# Arquitetura hexagonal para melhores microsserviços

![Honeybee](./_honeybee.png)

</div>

**Trilha:** Microservices (Recife e Online)

### Resumo

Exploraremos os benefícios do Domain Driven Development (DDD) e sua associação
com microsserviços e explorar o desenvolvimento com uma arquitetura hexagonal
utilizando ports e adaptors em microsserviços que permitem separar a lógica de
negócio de seus serviços.

O exemplo será em TypeScript, o que significa que será possível transferir o
conhecimento para outras linguagens e ainda que utilize AWS, um dos pontos
fortes é que a arquitetura hexagonal permite trocar para outras nuvens, para
outros serviços.

```ts
import { Handler } from "aws-lambda";

export const handler: Handler = async (event, _context) => {
  console.info(event);

  return {
    statusCode: 200,
  };
};
```
