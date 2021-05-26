---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dac582c0d91c4acb0225303dc019bd7699b7dbeb
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665242"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let childFolders = await client.api('/me/mailFolders/AAMkAGVmMDEzM/childFolders?includeHiddenFolders=true')
    .version('beta')
    .get();

```