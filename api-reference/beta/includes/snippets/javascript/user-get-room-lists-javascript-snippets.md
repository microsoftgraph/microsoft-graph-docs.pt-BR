---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ecd8776d521e84c950e9562b12ef3e8c412483c2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724305"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/findRoomLists')
    .version('beta')
    .get();

```