---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 106e0941939f2fb6136aec251b2a53496d7b801b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944582"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/b2xUserFlows/B2X_1_PartnerSignUp/identityProviders/Facebook-OAUTH/$ref')
    .version('beta')
    .delete();

```