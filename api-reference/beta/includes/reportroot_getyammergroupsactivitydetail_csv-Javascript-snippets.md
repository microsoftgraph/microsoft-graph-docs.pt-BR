---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 87970838fe8c64d852b0a134389b3d82e894b3d2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481860"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerGroupsActivityDetail(period='D7')')
    .version('beta')
    .get();

```