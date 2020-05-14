---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed8bbafbb37567e8834006a7119baf886c98d68f
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44218450"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/timeOffReasons')
    .get();

```