---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3060921e418909d368b80c156f1cc5e6c832ebaa
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616292"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{driveId}')
    .version('beta')
    .get();

```