---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0450243c20e7320cca43b04790927ab4cce0bda1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779451"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let dataPolicyOperation = await client.api('/dataPolicyOperations/{id}')
    .version('beta')
    .get();

```