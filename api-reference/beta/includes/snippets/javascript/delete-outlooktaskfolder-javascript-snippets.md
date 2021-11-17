---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a157ea75ff74e7ebcfcbc66f57b3e8562e6d209b00e8db927d1f2a74e9a65dc9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899491"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/outlook/taskFolders/AAMkADIyAAAhrbPXAAA=')
    .version('beta')
    .delete();

```