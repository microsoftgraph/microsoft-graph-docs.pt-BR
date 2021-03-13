---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97d0d2bcd6472e684b249aeeb19d8e772318b7e7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794419"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sectionGroup = {
  displayName: 'Section group name'
};

await client.api('/me/onenote/notebooks/{id}/sectionGroups')
    .version('beta')
    .post(sectionGroup);

```