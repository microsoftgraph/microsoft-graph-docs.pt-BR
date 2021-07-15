---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fabf7bc4b004cf02525042b5e17d09f3a01817f1
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439592"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userFlowIdentityProviders = await client.api('/identity/b2xUserFlows/B2X_1_Test/userflowIdentityProviders')
    .version('beta')
    .get();

```