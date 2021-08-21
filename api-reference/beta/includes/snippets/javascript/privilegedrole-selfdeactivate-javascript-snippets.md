---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e61322828daa361831ef6a7a0301dc273e3299c0df4a1644d3e4ca8f363fe54e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900219"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/privilegedRoles/{id}/selfDeactivate')
    .version('beta')
    .post();

```