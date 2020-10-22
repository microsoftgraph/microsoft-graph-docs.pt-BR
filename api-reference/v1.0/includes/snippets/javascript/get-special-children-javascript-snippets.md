---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57473cbb142913cac15f7cc69b15304a822415f3
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612185"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/special/{special-folder-name}/children')
    .get();

```