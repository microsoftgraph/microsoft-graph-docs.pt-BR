---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f7caf09975e59fb101f5bff6efec4c91188448eaf3af234fc8fd9f4723b7d846
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327008"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let legalHold = await client.api('/compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}')
    .version('beta')
    .get();

```