---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4054672845ae8df3dbf10dee4ead1f8843b43ecb7b8c40e500b542287de7c94a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100899"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/directory/deleteditems/microsoft.graph.group')
    .version('beta')
    .get();

```