---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2610acaaa192fd46ebc673126bbba4cd5a2c9466
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63527949"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/termsOfUse/agreements/0ec9f6a6-159d-4dd8-a563-1f0b5935e80b')
    .delete();

```