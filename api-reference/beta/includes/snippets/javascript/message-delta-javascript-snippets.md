---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2c1d2532f1f545d85dfd5720959aa8a07425a297
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610955"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/{id}/messages/delta')
    .version('beta')
    .get();

```