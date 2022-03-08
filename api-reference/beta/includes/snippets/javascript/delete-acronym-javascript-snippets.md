---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0d5ac107753dcb6c15ac3e077da0a345b991915d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338438"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/search/acronyms/{acronymsId}')
    .version('beta')
    .delete();

```