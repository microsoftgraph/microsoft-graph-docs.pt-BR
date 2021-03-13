---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9c7022ff6fb52b31be79192dda9da3a5e3cb084b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781041"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const emailAuthenticationMethod = {
  emailAddress: 'kim@contoso.com'
};

await client.api('/users/kim@contoso.com/authentication/emailMethods')
    .version('beta')
    .post(emailAuthenticationMethod);

```