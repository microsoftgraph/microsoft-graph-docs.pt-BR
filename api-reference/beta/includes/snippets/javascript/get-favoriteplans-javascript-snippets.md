---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 20f58672046e208b3c9bb2c97110496d968de89a7eb69da3afe7cdacea433870
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159358"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let favoritePlans = await client.api('/me/planner/favoritePlans')
    .version('beta')
    .get();

```