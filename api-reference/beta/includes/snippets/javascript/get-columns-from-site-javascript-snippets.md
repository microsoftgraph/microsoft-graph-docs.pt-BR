---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d01952c2041d7206dd61c1805dab2129455f2cd5
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200771"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let columns = await client.api('/sites/{site-id}/columns')
    .version('beta')
    .get();

```