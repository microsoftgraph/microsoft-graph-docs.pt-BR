---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3ae5ecc704ea8fd11ff91f5d96d32e7f6bb42e07
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202563"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let microsoftAuthenticatorMethods = await client.api('/users/sandeep@contoso.com/authentication/microsoftAuthenticatorMethods')
    .get();

```