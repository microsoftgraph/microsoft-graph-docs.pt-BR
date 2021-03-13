---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a511c7a44a6bf9e37617d801114fa2f352a46ae6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779841"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rejectedSenders = await client.api('/groups/{id}/rejectedSenders')
    .version('beta')
    .get();

```