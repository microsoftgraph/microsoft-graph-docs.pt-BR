---
description: Automatically generated file. DO NOT MODIFY
ms.openlocfilehash: 0a436605be85161733e9c6ca08cfcb2da27ae85f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49350458"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const servicePrincipal = {
  appId: "65415bb1-9267-4313-bbf5-ae259732ee12",
};

let res = await client.api('/servicePrincipals')
    .version('beta')
    .post(servicePrincipal);

```