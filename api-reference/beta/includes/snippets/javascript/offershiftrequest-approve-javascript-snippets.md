---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e76f7afd98a2ee660cf9326ad75a6af2f8e50690
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/09/2020
ms.locfileid: "40994941"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const approve = {
  message: "Approved!"
};

let res = await client.api('/teams/schedule/offerShiftRequests/approve')
    .version('beta')
    .post(approve);

```