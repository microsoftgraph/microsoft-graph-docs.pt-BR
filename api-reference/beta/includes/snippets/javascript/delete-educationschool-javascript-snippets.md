---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a23cd922028856979dd7c7226eec4e4b5d18d76e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604835"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/schools/10002')
    .version('beta')
    .delete();

```