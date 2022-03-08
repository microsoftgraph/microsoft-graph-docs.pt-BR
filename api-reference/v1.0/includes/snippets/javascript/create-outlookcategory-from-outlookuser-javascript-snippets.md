---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 590321f96ac895cc18445cab24d1ba9c17d73abd
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335945"
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