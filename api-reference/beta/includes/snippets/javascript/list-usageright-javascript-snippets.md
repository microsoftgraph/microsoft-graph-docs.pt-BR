---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2d8d4d2a50c9a9f8f9282a62bfda1ac2db038446
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179136"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{objectId}/usageRights')
    .version('beta')
    .filter('state in ('active', 'suspended') and serviceIdentifier in ('ABCD')')
    .get();

```