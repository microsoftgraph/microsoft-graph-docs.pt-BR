---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3fe0b759fdc8ea025d49ffad7c8e1ab2f990ae06
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439215"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}')
    .version('beta')
    .delete();

```