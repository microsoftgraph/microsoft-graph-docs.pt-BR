---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c994f0260f61a4bf213b34b063d5c208cd2cb63f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463506"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/pages/{id}')
    .version('beta')
    .delete();

```