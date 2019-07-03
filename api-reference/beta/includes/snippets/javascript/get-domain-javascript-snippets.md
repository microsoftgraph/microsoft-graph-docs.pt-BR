---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c18898eec9384fc38695006dd0f85717f067a2bb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476788"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/contoso.com')
    .version('beta')
    .get();

```