---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9d39c395c66d44326eb600a2ab92963ec448db9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443765"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  groupIds: [
    "groupIds-value"
  ]
};

let res = await client.api('/contacts/{id}/checkMemberGroups')
    .version('beta')
    .post(String);

```