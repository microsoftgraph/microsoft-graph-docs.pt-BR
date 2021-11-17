---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ada66c2bf9a4516d177cf05631baacdb03e77f832200c5c990a9a811d84ac437
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375878"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarGroup = {
  name: 'Personal events'
};

await client.api('/me/calendarGroups')
    .version('beta')
    .post(calendarGroup);

```