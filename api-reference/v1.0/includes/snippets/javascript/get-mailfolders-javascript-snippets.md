---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a604165b281286aa8e1f16bfd4a2b314e58f54ea
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604386"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders')
    .get();

```