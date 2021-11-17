---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52c4bd5cf6ba9b5a47ecd762e0f529720b295e70a5ac59e6da115d4ae4205686
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216866"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/servicePrincipals/delta')
    .version('beta')
    .get();

```