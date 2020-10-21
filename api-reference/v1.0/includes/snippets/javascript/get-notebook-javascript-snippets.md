---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d40a28f680ce21127f6b718bff8723850ec7811b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607974"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/notebooks/{id}')
    .get();

```