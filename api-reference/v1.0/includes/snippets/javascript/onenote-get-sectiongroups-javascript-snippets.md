---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 86b35258ead08937234902a0b304d232bf8e2406
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790081"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sectionGroups = await client.api('/me/onenote/sectionGroups')
    .get();

```