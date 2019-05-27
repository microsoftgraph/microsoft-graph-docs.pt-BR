---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f62830d67a9a05603cc2801ff9e494228f948fd3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475840"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tiIndicator = {
  additionalInformation: "additionalInformation-after-update",
  confidence: 42,
  description: "description-after-update",
};

let res = await client.api('/security/tiIndicators/{id}')
    .version('beta')
    .update({tiIndicator : tiIndicator});

```