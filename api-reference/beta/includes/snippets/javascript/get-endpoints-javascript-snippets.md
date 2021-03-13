---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2f6f9ee19d4be4c89d1c2f7d4588cc8ad531f4be
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800311"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let endpoints = await client.api('/print/services/{id}/endpoints')
    .version('beta')
    .get();

```