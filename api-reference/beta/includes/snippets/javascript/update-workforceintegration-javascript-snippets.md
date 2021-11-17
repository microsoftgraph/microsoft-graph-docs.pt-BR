---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 55417992c88477eaef429e1d7e7f388f2deb301da7d5405f941081d903e35540
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214586"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workforceIntegration = {
  displayName: 'displayName-value',
  apiVersion: 99,
  encryption: {
    protocol: 'protocol-value',
    secret: 'secret-value'
  },
  isActive: true,
  url: 'url-value',
  supports: 'supports-value'
};

await client.api('/teamwork/workforceIntegrations/{workforceIntegrationId}')
    .version('beta')
    .update(workforceIntegration);

```