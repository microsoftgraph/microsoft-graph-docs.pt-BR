---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8d7df821b5c0b863b36541c2c5e5e7ccccdda4c6c50638ed6b15a795b6c1b457
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273326"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemInsightsSettings = {
  disabledForGroup: 'edbfe4fb-ec70-4300-928f-dbb2ae86c981'
};

await client.api('/organization/{organizationId}/settings/itemInsights')
    .version('beta')
    .update(itemInsightsSettings);

```