---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8844763279a36b944abd290198add54f2fa95374
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536383"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)')
    .version('beta')
    .get();

```