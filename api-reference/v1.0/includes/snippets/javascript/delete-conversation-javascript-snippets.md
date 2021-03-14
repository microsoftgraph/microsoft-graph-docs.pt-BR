---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d5aaa52faa17a16dc9a5168a0fb2fbccf913e3da
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788238"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/conversations/{id}')
    .delete();

```