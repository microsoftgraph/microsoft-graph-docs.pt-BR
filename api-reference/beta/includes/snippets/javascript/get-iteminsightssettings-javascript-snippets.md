---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63540ecb06ba26b1af57a3e789861b4df740dbc92ba953096b2118102aa1ad08
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271947"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let itemInsightsSettings = await client.api('/organization/{organizationId}/settings/itemInsights')
    .version('beta')
    .get();

```