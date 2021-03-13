---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a222956b232bc71ba6c390624464f04559dd6ebf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785108"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subscription = await client.api('/me/drive/root/subscriptions/socketIo')
    .version('beta')
    .get();

```