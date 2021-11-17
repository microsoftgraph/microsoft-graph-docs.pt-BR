---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 012f3ffa095695cf3cbdbe4e588592e619ac433771b49ce7bbbd95e4aeb903ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217419"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/kim@contoso.com/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1')
    .version('beta')
    .delete();

```