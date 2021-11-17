---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 93b9377c5ea8cce4d1cddbb7e55a2f120dff6098c9f515c28a9dce2218c5b0f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274754"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let featureRolloutPolicy = await client.api('/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c')
    .version('beta')
    .get();

```