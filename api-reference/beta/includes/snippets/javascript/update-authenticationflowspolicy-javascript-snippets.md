---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9c3b8e11a9216bfcbd07b0f105ec0bfb3aea1f48378c65eb7f5c9192d9f254f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100172"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationFlowsPolicy = {
  selfServiceSignUp: {
    isEnabled: true
  }
};

await client.api('/policies/authenticationFlowsPolicy')
    .version('beta')
    .update(authenticationFlowsPolicy);

```