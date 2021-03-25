---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63d9a8beca98318dbb29bff539ff8e8488f1066c
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202737"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator')
    .delete();

```