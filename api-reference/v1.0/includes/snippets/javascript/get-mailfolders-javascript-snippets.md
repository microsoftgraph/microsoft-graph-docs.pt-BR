---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a604165b281286aa8e1f16bfd4a2b314e58f54ea
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507672"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders')
    .get();

```