---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c9e5467f04b9196173727dd61a7023dd9ffb4c15
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802249"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sectionGroup = await client.api('/me/onenote/sectionGroups/{id}')
    .version('beta')
    .get();

```