---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95344a67e0c09c9aef4f6768e3bb5fcb99c417c7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783940"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getSourceImages = await client.api('/deviceManagement/virtualEndpoint/deviceImages/getSourceImages')
    .version('beta')
    .get();

```