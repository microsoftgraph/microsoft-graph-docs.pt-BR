---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8fd569a55ee88abca1aff89a7e8f3adf6386b6ed
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785190"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/schools/10001/classes/11001')
    .version('beta')
    .delete();

```