---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 922eb2c4a640e6d0147c3cb33ed12e4ffb381042
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52266660"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let updatableAssets = await client.api('/admin/windows/updates/updatableAssets')
    .version('beta')
    .get();

```