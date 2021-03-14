---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6cf3dd842d7728af5d2a46c864a5f00294e6aa0f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800439"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/education/classes/{class-id}/group')
    .get();

```