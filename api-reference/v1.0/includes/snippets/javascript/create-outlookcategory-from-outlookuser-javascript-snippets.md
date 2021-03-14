---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c37bbf23bb28715c77b0fd0f3414043a0c1aea94
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788745"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookCategory = {
      displayName: 'Project expenses',
      color: 'preset9'
};

await client.api('/me/outlook/masterCategories')
    .post(outlookCategory);

```