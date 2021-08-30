---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 170d68d82356b3ce1d373fb46c04916798d812ae401347e053a340410a08bdb1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897997"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveMemberOf = await client.api('/servicePrincipals/{id}/transitiveMemberOf')
    .version('beta')
    .get();

```