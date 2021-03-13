---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b7e35223f080e77af8d4d9034f23d6361206030c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799583"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReview = {
    displayName: 'TestReview new name'
};

await client.api('/accessReviews/006111db-0810-4494-a6df-904d368bd81b')
    .version('beta')
    .update(accessReview);

```