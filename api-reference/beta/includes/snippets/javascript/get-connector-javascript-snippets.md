---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0fc44d101262cecfb837b37beca11a14d2caf730
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945287"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectors/{id}')
    .version('beta')
    .get();

```