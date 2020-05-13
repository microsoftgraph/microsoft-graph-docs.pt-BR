---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e238567d2ec1be53d2ec1878ee098d0b9bd70742
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "35725660"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/shifts')
    .version('beta')
    .filter('sharedShift/startDateTime ge 2019-03-11T00:00:00.000Z and sharedShift/endDateTime le 2019-03-18T00:00:00.000Z and draftShift/startDateTime ge 2019-03-11T00:00:00.000Z and draftShift/endDateTime le 2019-03-18T00:00:00.000Z')
    .get();

```