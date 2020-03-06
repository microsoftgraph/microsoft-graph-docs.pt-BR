---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d08f441a8dabd4a25fba100c6cf70e12aa0d2b45
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636475"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarGroup = {
  name: "name-value"
};

let res = await client.api('/me/calendarGroups/{id}')
    .update(calendarGroup);

```