---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3d0f956d5324e8ada5c0af667d59e8eb982c5f4aaa1ee128618c2cfb2c7e119e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101516"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/shares/{id}')
    .version('beta')
    .delete();

```