---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1c45b6685ce48f5d0f3255388cac83b0afe487b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498227"
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