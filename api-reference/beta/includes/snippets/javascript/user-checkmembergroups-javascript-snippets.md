---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d63ba97ad9376231971f3dae76fa1dc57b984cf3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716711"
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

let res = await client.api('/me/checkMemberGroups')
    .version('beta')
    .post(String);

```