---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 746071eb7acc7ab87964b7a384b5cb2e79ab7771
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873045"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources')
    .version('beta')
    .get();

```