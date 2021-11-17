---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7404e90c69b2f6dc7c6217abb79dfbb6bfa39b15
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "61007234"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignments = await client.api('/roleManagement/directory/roleAssignments')
    .version('beta')
    .filter(' principalId eq \'f1847572-48aa-47aa-96a3-2ec61904f41f\'')
    .get();

```