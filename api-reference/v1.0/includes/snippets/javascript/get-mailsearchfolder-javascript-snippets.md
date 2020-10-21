---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8c7a60acc5aeacfa557e2158c834dfd8b35a2c72
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615758"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/AAMkAGVmMDEzN')
    .get();

```