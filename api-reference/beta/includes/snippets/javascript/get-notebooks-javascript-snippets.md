---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e680000fb85346872df28891fcb082fbf26b9386
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620257"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/notebooks')
    .version('beta')
    .get();

```