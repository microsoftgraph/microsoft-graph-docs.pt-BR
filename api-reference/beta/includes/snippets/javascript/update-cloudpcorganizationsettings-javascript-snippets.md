---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0aa1fc523b15dd8739c8ed9574630f9d8ecf3266
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220194"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cloudPcOrganizationSettings = {
  '@odata.type': '#microsoft.graph.cloudPcOrganizationSettings',
  userAccountType: 'standardUser',
  osVersion: 'windows11',
  windowsSettings: {
    language: 'en-US'
  }
};

await client.api('/deviceManagement/virtualEndpoint/organizationSettings')
    .version('beta')
    .update(cloudPcOrganizationSettings);

```