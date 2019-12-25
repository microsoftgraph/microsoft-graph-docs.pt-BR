---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 45df2f8b000f50ca1012871250a3ce7f583280d8
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870571"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workforceIntegration = {
  displayName: "displayName-value",
  apiVersion: 99,
  encryption: {
    protocol: "protocol-value",
    secret: "secret-value"
  },
  isActive: true,
  url: "url-value",
  supports: "supports-value"
};

let res = await client.api('/teamwork/workforceIntegrations')
    .version('beta')
    .post(workforceIntegration);

```