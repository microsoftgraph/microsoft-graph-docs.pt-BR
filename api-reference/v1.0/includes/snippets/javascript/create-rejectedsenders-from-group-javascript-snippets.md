---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8907923c2af67da437aed8fa61a8b2bfabb99983
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636420"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id:"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
};

let res = await client.api('/groups/{id}/rejectedSenders/$ref')
    .post(directoryObject);

```