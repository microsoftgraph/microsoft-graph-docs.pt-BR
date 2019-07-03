---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 250ed8115374fd6eb7589d0868bcfe8f2215b61a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508806"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tentativelyAccept = {
  comment: "comment-value",
  sendResponse: true
};

let res = await client.api('/me/events/{id}/tentativelyAccept')
    .post(tentativelyAccept);

```