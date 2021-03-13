---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 26f246db38f8b8dd34eff4b829667ef8d63624c3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802299"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let agreementAcceptances = await client.api('/me/agreementAcceptances')
    .version('beta')
    .get();

```