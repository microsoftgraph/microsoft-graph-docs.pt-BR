---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 010460cffe29ebc051221b34e63ec0cbbf37b624
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806016"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getCredentialUserRegistrationCount = await client.api('/reports/getCredentialUserRegistrationCount')
    .version('beta')
    .get();

```