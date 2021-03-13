---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd940e697f30d39bef62213c0f2d2bb9a1af9b07
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805599"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getRelyingPartyDetailedSummary = await client.api('/reports/getRelyingPartyDetailedSummary(period='period_value')')
    .version('beta')
    .get();

```