---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06542a543bd1471cd45583317e3d18811629236a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508818"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists')
    .get();

```