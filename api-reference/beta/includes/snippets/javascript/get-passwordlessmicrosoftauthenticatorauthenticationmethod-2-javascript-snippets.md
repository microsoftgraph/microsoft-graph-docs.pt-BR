---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 74843a949e2c846d50b63084a2c287cf5afb9792b79a3d5bda7753a3527f5b7a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327636"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let passwordlessMicrosoftAuthenticatorMethods = await client.api('/me/authentication/passwordlessMicrosoftAuthenticatorMethods')
    .version('beta')
    .get();

```