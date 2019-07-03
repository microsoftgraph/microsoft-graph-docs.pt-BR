---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81a6f66b4f003303492f33e89385503fd4c34772
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477716"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/app/calls/{id}/audioRoutingGroups/{id}')
    .version('beta')
    .get();

```