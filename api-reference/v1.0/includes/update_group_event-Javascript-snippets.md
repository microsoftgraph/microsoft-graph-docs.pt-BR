---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1c9bc81f713a268d73888a3b86927986bb811650
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536768"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const event = {
  location:{
      displayName:"Conf Room 2"
  }
};

let res = await client.api('/groups/01d4ee64-15ce-491e-bad1-b91aa3223df4/calendar/events/AAMkADZlAAAAABERAAA=')
    .update({event : event});

```