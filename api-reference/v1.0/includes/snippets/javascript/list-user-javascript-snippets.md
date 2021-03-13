---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 752f35c25e06658d99992bdfb8d253fe3e23c75d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771537"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let allowedUsers = await client.api('/print/shares/{printerShareId}/allowedUsers')
    .get();

```