---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d13f5f65e560acaf01b1d05f550038ab46a8ae2ce948edb76d8311c51510fe22
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214759"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let microsoftAuthenticatorMethods = await client.api('/users/anirban@contoso.com/authentication/microsoftAuthenticatorMethods')
    .version('beta')
    .get();

```