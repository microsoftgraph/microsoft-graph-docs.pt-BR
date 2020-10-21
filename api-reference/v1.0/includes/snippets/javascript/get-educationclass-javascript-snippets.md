---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a764022f5cdd42f6a51e8b18d2e56cc18ccfac93
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611140"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/{class-id}')
    .get();

```