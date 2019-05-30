---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0123bec184b2f1f0145b109bef7016ec6a9856d4
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536628"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)')
    .get();

```