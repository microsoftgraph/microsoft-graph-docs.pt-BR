---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37aae13c03f8a188b6f35f266213ec4370496b5a
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475595"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodConfiguration = {
    @odata.type: "#microsoft.graph.smsAuthenticationMethodConfiguration",
    id: "Sms",
    state: "enabled"
};

let res = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms')
    .version('beta')
    .update(authenticationMethodConfiguration);

```