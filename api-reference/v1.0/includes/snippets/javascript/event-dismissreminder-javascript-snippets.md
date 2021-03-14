---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc1fd3683a08d4d475a2752eb310b871cf595df9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802534"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/events/{id}/dismissReminder')
    .post();

```