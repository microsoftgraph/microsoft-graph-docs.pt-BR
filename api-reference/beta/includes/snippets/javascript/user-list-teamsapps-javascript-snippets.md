---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7d1167beca9d61061055cfbc9980bda7d4c71a8
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945379"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/teamwork/installedApps/{id}')
    .version('beta')
    .get();

```