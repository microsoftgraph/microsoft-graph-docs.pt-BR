---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3d4848be6ea03b83272c08d28a38b294b45c1078
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437297"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryObjects/delta')
    .version('beta')
    .filter('isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')')
    .get();

```