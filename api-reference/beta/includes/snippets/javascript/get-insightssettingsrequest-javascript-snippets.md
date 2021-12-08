---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d3a77991a070286553af547968007039885b26fa
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61343708"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let insightsSettings = await client.api('/organization/{organizationId}/settings/itemInsights')
    .version('beta')
    .get();

```