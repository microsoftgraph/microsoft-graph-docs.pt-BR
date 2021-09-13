---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 234b600119651a7ce252eee45135aab9f73dd34954882f0d75cc6fb7e308f087
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101065"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/renew')
    .post();

```