---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f0bc18c79feadf321f032c1a90e130fa4ac8a8fb
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338026"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRbacResourceAction = await client.api('/roleManagement/directory/resourceNamespaces/microsoft.directory/resourceActions/microsoft.directory-accessReviews-allProperties-read-get')
    .version('beta')
    .get();

```