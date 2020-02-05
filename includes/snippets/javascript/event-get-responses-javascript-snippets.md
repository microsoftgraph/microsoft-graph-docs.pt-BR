---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17f3d66d9efaf16dc0128588e6f362981e6e9321
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774626"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendar/events/AAMkADJXJGu0AABf02qwAAA=')
    .get();

```