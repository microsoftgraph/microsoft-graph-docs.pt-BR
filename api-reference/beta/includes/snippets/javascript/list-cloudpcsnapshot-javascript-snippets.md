---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae42294da71a5599ba8b5ad50d311d8e65216619
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335343"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let snapshots = await client.api('/deviceManagement/virtualEndpoint/snapshots')
    .version('beta')
    .get();

```