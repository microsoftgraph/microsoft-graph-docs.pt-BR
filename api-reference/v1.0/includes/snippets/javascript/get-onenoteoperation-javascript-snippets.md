---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 759c2016343a4c26e9a9723735ba2cb1000838b4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789795"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onenoteOperation = await client.api('/me/onenote/operations/{id}')
    .get();

```