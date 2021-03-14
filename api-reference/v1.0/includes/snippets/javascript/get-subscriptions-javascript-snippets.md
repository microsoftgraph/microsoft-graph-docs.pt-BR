---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2aa88bbb61cfeb3904675ee472d9e12b225efa73
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780138"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subscriptions = await client.api('/subscriptions')
    .get();

```