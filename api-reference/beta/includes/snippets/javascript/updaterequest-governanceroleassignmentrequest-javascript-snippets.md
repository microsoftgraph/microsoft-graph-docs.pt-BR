---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a64e3577ae989df007a3186cc95dd538acc18451d8eab90292f0bce0a629cd39
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215374"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest')
    .version('beta')
    .post();

```