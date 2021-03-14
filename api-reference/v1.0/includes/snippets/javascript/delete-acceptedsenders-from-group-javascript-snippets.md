---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 952ecf89ff3220558c0b610cd7207811ca29dfbf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778702"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/acceptedSenders/$ref')
    .delete();

```