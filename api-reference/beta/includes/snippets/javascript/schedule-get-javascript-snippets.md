---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37a2658d9c4dcb30632ed49d2ac10cc5fd3afbd1
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "35718242"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule')
    .version('beta')
    .get();

```