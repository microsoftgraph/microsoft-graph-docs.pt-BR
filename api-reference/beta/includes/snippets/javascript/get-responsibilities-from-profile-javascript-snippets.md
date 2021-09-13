---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2a9c5dfd86a356a050f575691df431dfb6b66bd5a77ef1716485fe660187a36
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329377"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let responsibilities = await client.api('/me/responsibilities')
    .version('beta')
    .get();

```