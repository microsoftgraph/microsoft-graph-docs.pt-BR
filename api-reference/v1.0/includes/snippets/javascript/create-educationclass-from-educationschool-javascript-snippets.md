---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bda07ec460cd81b27d76ae0978a3caa365a5711d
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015844"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/schools/{school-id}/users/{user-id}')
    .delete();

```