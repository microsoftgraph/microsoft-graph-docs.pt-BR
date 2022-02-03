---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0db9086697ebd0fde5692e6a4b52c31e9eb6c11
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348374"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const updateSoftware = {
  softwareType: 'teamsClient',
  softwareVersion: '1.0.96.22'
};

await client.api('/teamwork/devices/0f3ce432-e432-0f3c-32e4-3c0f32e43c0f/updateSoftware')
    .version('beta')
    .post(updateSoftware);

```