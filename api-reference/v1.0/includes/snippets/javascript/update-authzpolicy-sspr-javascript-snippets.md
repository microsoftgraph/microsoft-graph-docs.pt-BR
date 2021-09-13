---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 985168bf2271c0478c7b8536b735721d2c5a5dcb55d15d17d5b6e85d8fa2d413
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272828"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
   allowedToUseSSPR: true
};

await client.api('/policies/authorizationPolicy')
    .update(authorizationPolicy);

```