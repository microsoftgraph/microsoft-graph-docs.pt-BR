---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd9724cd445c696af86e247255194c978e423eb5
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346004"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let insightsSettings = await client.api('/organization/{organizationId}/settings/peopleInsights')
    .version('beta')
    .get();

```