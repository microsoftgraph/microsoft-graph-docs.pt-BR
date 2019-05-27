---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 64d4527a598c9c0b8770c554e7fe8dfdc585dfe4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462877"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}/items')
    .get();

```