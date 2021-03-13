---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 783b4ef80c5bd153803978ac018bdb183efa8e6b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781457"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const checkin = {
  comment: 'Updating the latest guidelines'
};

await client.api('/drives/{drive-id}/items/{item-id}/checkin')
    .version('beta')
    .post(checkin);

```