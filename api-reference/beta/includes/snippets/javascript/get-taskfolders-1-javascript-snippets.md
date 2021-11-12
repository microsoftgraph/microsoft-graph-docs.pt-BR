---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a3fa8770a2756efdfb8d7bbbec8a7a4a7cde80576bf1bf7c65f971cf8ec81b51
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159373"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let taskFolders = await client.api('/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=/taskFolders')
    .version('beta')
    .get();

```