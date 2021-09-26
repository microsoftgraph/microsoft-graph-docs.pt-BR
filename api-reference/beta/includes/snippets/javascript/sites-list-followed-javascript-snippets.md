---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3027aca3d3d117bf0841cf431c83b92f9fd30395cac3b2e5de93b08e979cf16
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217297"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let followedSites = await client.api('/me/followedSites')
    .version('beta')
    .get();

```