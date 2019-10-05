---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 32e3937a2fe48693307ec36f5540e9fe72fe02c9
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402470"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites')
    .version('beta')
    .filter('siteCollection/root ne null')
    .select('siteCollection,webUrl')
    .get();

```