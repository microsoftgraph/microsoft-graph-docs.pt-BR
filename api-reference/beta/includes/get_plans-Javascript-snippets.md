---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 551da0259c67eced0dad5ea40875c573b00584a9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447576"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/planner/plans')
    .version('beta')
    .get();

```