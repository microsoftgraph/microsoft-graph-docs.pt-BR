---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 691c661fa4f7f2dadf9c52e9845034e8b6d90564
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787968"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let childFolders = await client.api('/me/contactFolders/{id}/childFolders')
    .get();

```