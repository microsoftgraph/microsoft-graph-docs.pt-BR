---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7dc9500cb4bff356a3a85a6bbc714405d37e8e2a
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015412"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/{class-id}/schools')
    .get();

```