---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 179b124b421c65dc2809f4c455e2c096a354587c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612532"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/supportedLanguages')
    .version('beta')
    .get();

```