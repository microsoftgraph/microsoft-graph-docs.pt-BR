---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a8f0f053b12fa2265fb4f873101c1018e333caa2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783609"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const event = {
  location: {
      displayName: 'Conf Room 2'
  }
};

await client.api('/groups/01d4ee64-15ce-491e-bad1-b91aa3223df4/calendar/events/AAMkADZlAAAAABERAAA=')
    .update(event);

```