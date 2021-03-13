---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dbc5ce44d17c01d4fb0e4439e09a7ac2538b19d6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781738"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let overrides = await client.api('/me/inferenceClassification/overrides')
    .version('beta')
    .get();

```