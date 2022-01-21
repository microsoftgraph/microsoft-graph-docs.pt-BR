---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6abfbc28a1e0bea30d080d8f6f7d5755fa4b21f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088230"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskDetection = await client.api('/identityProtection/riskDetections/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3')
    .get();

```