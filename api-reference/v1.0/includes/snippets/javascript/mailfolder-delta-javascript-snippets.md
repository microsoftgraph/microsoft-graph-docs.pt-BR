---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63ee4963e5e8844cfbf7d45e637200c8d47907cd
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605784"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/delta')
    .get();

```