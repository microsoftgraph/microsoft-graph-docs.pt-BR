---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb63969d015ad5dbc91825e0c52e291b2ec70f1d
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668574"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contentTypes = await client.api('/sites/{site-id}/lists/{list-id}/contentTypes')
    .version('beta')
    .get();

```