---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 687bbe11a3fa234f21e406fc709e3694d55cf912
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439152"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/')
    .version('beta')
    .delete();

```