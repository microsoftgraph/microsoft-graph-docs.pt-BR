---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 575d8606f0d966e09840c35be69125c7b547585749255ee6cf7ee12934b9d2ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214154"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/calendarGroups/{id}')
    .version('beta')
    .delete();

```