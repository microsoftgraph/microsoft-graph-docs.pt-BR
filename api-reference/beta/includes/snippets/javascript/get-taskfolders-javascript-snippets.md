---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2edaab62f16939eec92a4e16e39d44af332609e
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015107"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=/taskFolders')
    .version('beta')
    .get();

```