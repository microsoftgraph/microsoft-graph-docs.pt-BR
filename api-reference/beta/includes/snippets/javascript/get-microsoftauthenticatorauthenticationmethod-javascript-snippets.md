---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1373e073b179ccf0cd2e8429e097bb3dc697124d63470e35127ed72e34820b87
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157078"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let microsoftAuthenticatorAuthenticationMethod = await client.api('/users/anirban@contoso.com/authentication/microsoftAuthenticatorMethods/_jpuR-TGZtk6aQCLF3BQjA2')
    .version('beta')
    .get();

```