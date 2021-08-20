---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6946f48795b9c07ce7fafccd742ab799bbc31278
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259098"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let healthOverviews = await client.api('/admin/serviceAnnouncement/healthOverviews')
    .get();

```