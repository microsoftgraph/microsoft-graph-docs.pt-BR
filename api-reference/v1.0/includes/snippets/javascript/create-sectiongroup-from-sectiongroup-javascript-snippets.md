---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7fc7af8234b0aaef15acbf3723346db0fbc9881
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789289"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sectionGroup = {
  displayName: 'Section group name'
};

await client.api('/me/onenote/sectionGroups/{id}/sectionGroups')
    .post(sectionGroup);

```