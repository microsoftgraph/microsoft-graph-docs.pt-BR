---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21758f0773c11184a7f9019167fb9420cca6dded
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945216"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/offerShiftRequests')
    .version('beta')
    .get();

```