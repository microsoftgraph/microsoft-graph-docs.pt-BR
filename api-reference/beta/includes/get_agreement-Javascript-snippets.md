---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd0fcd02bf174e1058ae5be8f40f81dcef4a2191
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474209"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/agreements/'id'')
    .version('beta')
    .expand('files')
    .get();

```