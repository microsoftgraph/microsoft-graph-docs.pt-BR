---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 74544f295b517be5ce7773301a9c292a0d0a9919069dc0f74ecb62c7a4527b94
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216121"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/b2xUserFlows/B2X_1_PartnerSignUp/identityProviders/Facebook-OAUTH/$ref')
    .delete();

```