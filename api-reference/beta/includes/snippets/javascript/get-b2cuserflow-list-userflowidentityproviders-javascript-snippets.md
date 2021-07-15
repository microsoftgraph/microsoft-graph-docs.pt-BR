---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 250d90a3d5a0f67ed21c6d3e6f9cfa50d747dd2a
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439740"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userFlowIdentityProviders = await client.api('/identity/b2cUserFlows/B2C_test_signin_signup/userflowIdentityProviders')
    .version('beta')
    .get();

```