---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9f10a658bc0b6ddbf4f53200370ba818abe905ae
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61339492"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const insightsSettings = {
  disabledForGroup: 'edbfe4fb-ec70-4300-928f-dbb2ae86c981'
};

await client.api('/organization/{organizationId}/settings/itemInsights')
    .version('beta')
    .update(insightsSettings);

```