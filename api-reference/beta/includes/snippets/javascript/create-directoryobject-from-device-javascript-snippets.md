---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b092d260da73320978f803e5098cedffb09f34c5
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/beta/directoryObjects/{id}"
};

let res = await client.api('/devices/{id}/registeredOwners/$ref')
    .version('beta')
    .post(directoryObject);

```