---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96775ea532d54d332be67ff20b07aa7f8ca1d476e4770be48ba2301ec7ab083d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214369"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let microsoftAuthenticatorMethods = await client.api('/users/sandeep@contoso.com/authentication/microsoftAuthenticatorMethods')
    .get();

```