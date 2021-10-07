---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 028a004e5a945f9efdbe74fb525e34c5876c6b0709feda8341b57d90563f1418
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160246"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationMethodConfiguration = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator')
    .version('beta')
    .get();

```