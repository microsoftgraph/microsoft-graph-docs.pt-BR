---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f5c668d8830c3aad241665501b556959af8bbafa
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472462"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator')
    .version('beta')
    .delete();

```