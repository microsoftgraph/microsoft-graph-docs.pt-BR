---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1a2d3fafabbaccf1e273ec026a6ff979f3a01a13
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658903"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const custodian = {
  applyHoldToSources: "false",
};

let res = await client.api('/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239')
    .version('beta')
    .update(custodian);

```