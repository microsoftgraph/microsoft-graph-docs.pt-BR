---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 14769cda26b1ba5d7b3813c46c1c71235b131c62
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015370"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes')
    .get();

```