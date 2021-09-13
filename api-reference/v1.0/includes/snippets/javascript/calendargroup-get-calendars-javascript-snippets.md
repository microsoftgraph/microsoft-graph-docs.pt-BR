---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6326d913b2f0bd94d07b966459f43ed12db3e06dafd862d701e09161da73604f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272814"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendars = await client.api('/me/calendarGroups/{id}/calendars')
    .get();

```