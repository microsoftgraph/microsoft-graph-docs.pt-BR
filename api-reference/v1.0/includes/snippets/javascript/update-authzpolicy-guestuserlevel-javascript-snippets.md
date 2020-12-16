---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c003aab74c569fd9e9e92e3015cfecd3e817b815
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691379"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
  allowEmailVerifiedUsersToJoinOrganization:false
};

let res = await client.api('/policies/authorizationPolicy')
    .update(authorizationPolicy);

```