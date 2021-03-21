---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f0f1c43b5498df58fb2602e9d98b70fada74d917
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960145"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let namedLocations = await client.api('/identity/conditionalAccess/namedLocations')
    .filter('createdDateTime ge 2019-09-01T00:00:00Z')
    .get();

```