---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3616918779657d3ca123fc1c82e801efa0ee2acb
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638679"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/organization/{id}/certificateBasedAuthConfiguration')
    .get();

```