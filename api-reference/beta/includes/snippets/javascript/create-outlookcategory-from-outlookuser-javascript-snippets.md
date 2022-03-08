---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 823e0c95d7769a4b1f77b56cc61a620b68d17326
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333740"
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
    .version('beta')
    .post(outlookCategory);

```