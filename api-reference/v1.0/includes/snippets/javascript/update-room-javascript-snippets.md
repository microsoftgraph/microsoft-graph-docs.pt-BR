---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1bae41f75ccbfe6a1e14c7f991843a25b565d4d0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808672"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const place = {
  '@odata.type': 'microsoft.graph.room',
  nickname: 'Conf Room',
  building: '1',
  label: '100',
  capacity: 50,
  isWheelChairAccessible: false
};

await client.api('/places/cf100@contoso.com')
    .update(place);

```