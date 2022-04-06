---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e85fe986fb0b1e336e5be2b2492082f9cc90c4df
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516179"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let agreement = await client.api('/identityGovernance/termsOfUse/agreements/093b947f-8363-4979-a47d-4c52b33ee1be')
    .version('beta')
    .expand('files')
    .get();

```