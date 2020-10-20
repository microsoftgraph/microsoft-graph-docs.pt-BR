---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18ca20629964f013af43a53d655ae9bd05491b78
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606253"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains')
    .version('beta')
    .get();

```