---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5764e58463273ad4209bc24111bd26fa2265765550868bb4bc60a97b51f07819
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214624"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile')
    .version('beta')
    .delete();

```