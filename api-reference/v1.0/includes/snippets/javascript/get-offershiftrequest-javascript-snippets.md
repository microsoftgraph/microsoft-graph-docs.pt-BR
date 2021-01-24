---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e65075cf5ca357f6c4c2fbad959b24b91bb1b7a2
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946247"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/offerShiftRequests')
    .get();

```