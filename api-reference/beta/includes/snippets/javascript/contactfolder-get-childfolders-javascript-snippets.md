---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 41ca2b4ea3c7e8df8b476aa49bf3500fb71227c6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799713"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let childFolders = await client.api('/me/contactFolders/{id}/childFolders')
    .version('beta')
    .get();

```