---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: daceffe89c908f9bfb6562b8f3ec57dc6e817499
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444395"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites')
    .version('beta')
    .filter('siteCollection/root ne null')
    .get();

```