---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9e12670caaa15b33d78ce1294e7b48a2ce64fb1
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610376"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contracts')
    .version('beta')
    .get();

```