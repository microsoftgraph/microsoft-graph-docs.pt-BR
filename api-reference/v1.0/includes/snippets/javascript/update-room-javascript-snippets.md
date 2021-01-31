---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d26fc85416d88a2ec2e4bc614c4a9a68726ddc13
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059616"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const place = {
  @odata.type: "microsoft.graph.room",
  nickname: "Conf Room",
  building: "1",
  label: "100",
  capacity: 50,
  isWheelChairAccessible: false
};

let res = await client.api('/places/cf100@contoso.com')
    .update(place);

```