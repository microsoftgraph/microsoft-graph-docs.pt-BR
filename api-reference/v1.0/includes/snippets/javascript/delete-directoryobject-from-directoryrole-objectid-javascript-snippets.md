---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 847db859099070f2ab346b0afb48a40d0213f8f6
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522792"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/{role-objectId}/members/{user-id}/$ref')
    .delete();

```