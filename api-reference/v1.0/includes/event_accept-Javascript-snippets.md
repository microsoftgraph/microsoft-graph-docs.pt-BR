---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 901d71545e8156cde08a1481f6950997a15daebd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457821"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accept = {
  comment: "comment-value",
  sendResponse: true
};

let res = await client.api('/me/events/{id}/accept')
    .post(accept);

```