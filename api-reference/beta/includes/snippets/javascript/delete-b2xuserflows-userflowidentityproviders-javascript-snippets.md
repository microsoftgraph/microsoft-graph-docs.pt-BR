---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 192cf383c9f858447d83a08ea9a21fa89d7e0434
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439642"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/b2cUserFlows/B2C_test_signin_signup/userflowIdentityProviders/MSA-OIDC/$ref')
    .version('beta')
    .delete();

```