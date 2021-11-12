---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76083ba64ef29efe48054661438ca1ab9df76126e30ad1e52283307e7cdbdf2e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156343"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendars = await client.api('/me/calendarGroups/{id}/calendars')
    .version('beta')
    .get();

```