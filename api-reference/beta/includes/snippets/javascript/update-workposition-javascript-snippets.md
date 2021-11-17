---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59e9da9c20f41e4f3af273149ea1dc969d7449b8504bea0965ef7ff05c6653a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101915"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workPosition = {
  isCurrent: true
};

await client.api('/me/profile/positions/{id}')
    .version('beta')
    .update(workPosition);

```