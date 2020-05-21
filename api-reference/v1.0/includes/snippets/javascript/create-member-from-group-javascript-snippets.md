---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8641059c4adeb886bb278146b0b8129fe1490175
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636422"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
};

let res = await client.api('/groups/{id}/members/$ref')
    .post(directoryObject);

```