---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98a283d93273c4f00265041e123f80781641582c
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2020
ms.locfileid: "45224616"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}/registeredOwners/{id}/$ref')
    .delete();

```