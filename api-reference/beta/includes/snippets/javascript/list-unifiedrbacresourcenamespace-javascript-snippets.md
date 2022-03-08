---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8bb48716c882b6c293a8956d091904bc66cc53f3
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338125"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let resourceNamespaces = await client.api('/roleManagement/directory/resourceNamespaces')
    .version('beta')
    .get();

```