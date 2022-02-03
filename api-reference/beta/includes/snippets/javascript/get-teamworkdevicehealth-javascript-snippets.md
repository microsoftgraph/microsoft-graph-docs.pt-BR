---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 941143462fb40d29bbf1b2022b8653daa4c1972a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349014"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamworkDeviceHealth = await client.api('/teamwork/devices/d8214fe3-4fe3-d821-e34f-21d8e34f21d8/health')
    .version('beta')
    .get();

```