---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 101e6b522909a2c7ab66c53a7149c6487612f55b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618059"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/{id}/scopedMembers')
    .version('beta')
    .get();

```