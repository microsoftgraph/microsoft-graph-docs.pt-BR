---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18e9c0c350eb5adeb3bcd9e6979994314428c693
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616246"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/activities/recent')
    .get();

```