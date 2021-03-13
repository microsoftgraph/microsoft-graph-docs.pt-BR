---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e175406324462b7e08922a2fdf473230a584c1ed
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800397"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let childFolders = await client.api('/me/mailFolders/searchfolders/childFolders')
    .version('beta')
    .get();

```