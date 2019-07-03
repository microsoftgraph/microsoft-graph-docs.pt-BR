---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43915ed94ba5ba944e634d99c31a084fe76935b9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492125"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{drive-id}')
    .get();

```