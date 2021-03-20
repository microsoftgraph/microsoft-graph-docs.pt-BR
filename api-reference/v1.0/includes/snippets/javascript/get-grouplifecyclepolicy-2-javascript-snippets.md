---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af2e6f13cda16d48465a98360a2eec7d0c39ecf3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949873"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupLifecyclePolicies = await client.api('/groupLifecyclePolicies')
    .get();

```