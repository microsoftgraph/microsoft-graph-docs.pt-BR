---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 965e94329cce9444575cf860c9e0306268bee224f273b9b8cf7f736a12f93957
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329306"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  businessPhones: [
    '+1 425 555 0109'
  ],
  officeLocation: '18/2111'
};

await client.api('/users/{id}')
    .version('beta')
    .update(user);

```