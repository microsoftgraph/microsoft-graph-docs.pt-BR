---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00ae9b5bef1de1208b593df35616b4beae28262c989b2716d3820ae264221d98
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214236"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarGroup = {
  name: 'name-value'
};

await client.api('/me/calendarGroups/{id}')
    .version('beta')
    .update(calendarGroup);

```