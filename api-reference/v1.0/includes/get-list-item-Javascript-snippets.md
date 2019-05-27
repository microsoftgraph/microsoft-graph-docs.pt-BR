---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 122f972136b8f2853048d85f970270da54d316a7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470869"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}')
    .get();

```