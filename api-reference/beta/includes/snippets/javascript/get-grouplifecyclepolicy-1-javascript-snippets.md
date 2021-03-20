---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60cb46cf37c292c1c70a574eccf470c4442fd3ca
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944183"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupLifecyclePolicy = await client.api('/groupLifecyclePolicies/{id}')
    .version('beta')
    .get();

```