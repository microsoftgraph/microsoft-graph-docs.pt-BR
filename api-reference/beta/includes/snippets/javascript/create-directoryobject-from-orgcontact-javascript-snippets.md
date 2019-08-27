---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7559f58995cee52d7188753d961a336dbf49842b
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636246"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  directoryObject: {
  }
};

let res = await client.api('/contacts/{id}/memberOf')
    .version('beta')
    .post(directoryObject);

```