---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab1ae3436216b539c8f12975934d91ad643fa410
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787237"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let mailFolder = await client.api('/me/mailFolders/AAMkAGVmMDEzM')
    .version('beta')
    .get();

```