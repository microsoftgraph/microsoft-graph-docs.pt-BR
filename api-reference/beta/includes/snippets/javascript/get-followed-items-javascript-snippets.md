---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b903c65608c5b61d0c148cdb753a95683dbcd90a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519306"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/following')
    .version('beta')
    .get();

```