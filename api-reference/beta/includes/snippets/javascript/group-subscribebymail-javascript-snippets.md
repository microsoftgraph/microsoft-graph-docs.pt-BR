---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 646495da7db646d6834f0c53dedadca4f3488c2d3c11c1ff25bbde8de59e4f9c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101596"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/subscribeByMail')
    .version('beta')
    .post();

```