---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13e3678f8870c662bb1abbfd684787722ee310cc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889123"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/memberOf')
    .get();

```