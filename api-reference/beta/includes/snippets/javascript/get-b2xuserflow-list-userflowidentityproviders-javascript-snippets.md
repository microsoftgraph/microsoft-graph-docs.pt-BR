---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 004fc6dc316af304e1b25ff5c5d2e16ebbe35bcb139ad455df48f26fadb5d0a8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157673"
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