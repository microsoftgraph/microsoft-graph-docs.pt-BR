---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf3c4a9da4ddb9d3bf3ff65c49546fb113dfa5ba12ffa9b0ddc31bf56184c6a9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158963"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let homeRealmDiscoveryPolicies = await client.api('/policies/homeRealmDiscoveryPolicies')
    .get();

```