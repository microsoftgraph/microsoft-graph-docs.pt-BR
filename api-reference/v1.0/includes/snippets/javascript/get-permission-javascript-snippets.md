---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f26c569bef9b4f6bc007dd50ad3613cab2548e91
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808132"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permission = await client.api('/sites/{sitesId}/permissions/{permissionId}')
    .get();

```