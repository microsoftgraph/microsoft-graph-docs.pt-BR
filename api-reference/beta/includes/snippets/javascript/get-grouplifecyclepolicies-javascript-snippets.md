---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 257eb4eedbbebdd5e8601dd30c95bd0c28900d33ff94087c7d0eb816d6bbebaf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213803"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupLifecyclePolicies = await client.api('/groups/{id}/groupLifecyclePolicies')
    .version('beta')
    .get();

```