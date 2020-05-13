---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 88c8ef62b3ccbd9ae5fac1950f0b3340097f671f
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "35716830"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/timesOff/{timeOffId}')
    .version('beta')
    .delete();

```