---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ebf373caf96f7a4b714e6cb4e42e6aeb8e9057e5
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015580"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/todo/lists')
    .get();

```