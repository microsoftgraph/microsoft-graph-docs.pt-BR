---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 053cbd4bec431dde3868ab2141a0cdc900b9922899f1ffec3ea0fa66714c0e5b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272545"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let taskFolders = await client.api('/me/outlook/taskFolders')
    .version('beta')
    .get();

```