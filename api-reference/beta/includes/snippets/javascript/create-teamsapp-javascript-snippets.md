---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b619901e3dc3d616ce8d4091ff1e748551cced3a
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "48903543"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appCatalogs/teamsApps?requiresReview=true')
    .version('beta')
    .post();

```