---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1c45b6685ce48f5d0f3255388cac83b0afe487b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34482155"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerGroupsActivityGroupCounts(period='D7')')
    .version('beta')
    .get();

```