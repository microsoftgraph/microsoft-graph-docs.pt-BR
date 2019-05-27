---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e0c692776d86b734b2d8b93083f083d22dfd047f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459246"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/contoso.com')
    .delete();

```