---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 99aef51fb767f8e8c8b5567a536afdaad82967dd2f3c5ac46fa1a1076d855200
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100683"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendar = {
  name: 'Social events'
};

await client.api('/me/calendar')
    .update(calendar);

```