---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 87f1dcac48f054eba43ed7f8b81516cb40de823c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786182"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}')
    .delete();

```