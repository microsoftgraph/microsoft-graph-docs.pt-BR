---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00b02d3abdeb67c00905e72687cd83205d565ff9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474027"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/{id}')
    .version('beta')
    .get();

```