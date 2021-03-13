---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 313519314cfb70f21649f26c7887fd0d1c40f4c3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794090"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let listItem = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields')
    .version('beta')
    .get();

```