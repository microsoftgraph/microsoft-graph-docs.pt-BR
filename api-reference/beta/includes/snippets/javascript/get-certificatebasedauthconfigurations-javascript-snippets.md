---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a303a04f2badc6246e3060328e9d14eff463daf828d26ff4479daa2774ba7fc3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100576"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let certificateBasedAuthConfiguration = await client.api('/organization/{id}/certificateBasedAuthConfiguration')
    .version('beta')
    .get();

```