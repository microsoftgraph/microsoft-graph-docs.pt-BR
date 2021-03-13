---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b70e6a85679bc9e2f111c8c42cbba9b1d4cb9c5d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781103"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let pendingAccessReviewInstances = await client.api('/me/pendingAccessReviewInstances')
    .version('beta')
    .expand('definition')
    .skip(0)
    .top(100)
    .get();

```