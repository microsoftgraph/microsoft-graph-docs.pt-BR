---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7e2766cca2c2cff2b9ff2007d5557d525bb3fc31
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48622319"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/timeOffReasons')
    .version('beta')
    .get();

```