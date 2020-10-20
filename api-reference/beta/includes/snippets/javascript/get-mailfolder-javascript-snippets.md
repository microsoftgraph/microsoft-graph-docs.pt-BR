---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71043814d9b930ebc10679fd7c0d0ebc71c203cc
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605505"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/AAMkAGVmMDEzM')
    .version('beta')
    .get();

```