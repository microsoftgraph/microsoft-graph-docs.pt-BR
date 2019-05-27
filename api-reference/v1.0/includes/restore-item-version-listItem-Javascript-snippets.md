---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd4d4a8a230321c7e8e4d4db18c9c37d95c88feb
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470680"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion')
    .post();

```