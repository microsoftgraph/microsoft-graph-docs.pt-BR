---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 195d1def311b7307b19f26b355787c372796280f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518946"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerActivityUserDetail(period='D7')')
    .version('beta')
    .get();

```