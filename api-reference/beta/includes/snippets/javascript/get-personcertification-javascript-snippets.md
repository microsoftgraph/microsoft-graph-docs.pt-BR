---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 58990bfc7a9c0a04846cccfd505aebf41f500cce
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809954"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let personCertification = await client.api('/me/profile/certifications/{id}')
    .version('beta')
    .get();

```