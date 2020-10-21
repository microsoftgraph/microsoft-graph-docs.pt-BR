---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0603466429547d504e296fbd7d6061b96d6ae67
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615786"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{userId}/drives')
    .get();

```