---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5d24e680c62ba842fe25a3d32463c0faec42c527f6940729ae02a42b1589b268
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215356"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=/tasks')
    .version('beta')
    .get();

```