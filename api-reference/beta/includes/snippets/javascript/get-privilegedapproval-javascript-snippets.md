---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: edf92b8ae5faace33e8ad3ac983931baca01be79
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463342"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedApproval')
    .version('beta')
    .get();

```