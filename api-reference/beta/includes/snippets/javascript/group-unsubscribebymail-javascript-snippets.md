---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1058a230b5951dad2c7473933c17560f5d485626
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498859"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/unsubscribeByMail')
    .version('beta')
    .post();

```