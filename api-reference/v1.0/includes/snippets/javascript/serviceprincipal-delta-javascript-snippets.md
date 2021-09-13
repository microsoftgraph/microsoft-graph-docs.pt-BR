---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2275b9c42fa148d90d7bb86df382ce57b635c168854764ae8296cc74918054c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157905"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/servicePrincipals/delta')
    .get();

```