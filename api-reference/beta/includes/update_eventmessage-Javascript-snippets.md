---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af9a996eb8d2abc2b825263d687fa1217d4668ef
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34479375"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  isRead: "true",
};

let res = await client.api('/me/messages/{id}')
    .version('beta')
    .update({message : message});

```