---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab6ff611b215cbdf05d29ab57ed6ad017ce8d265
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962963"
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