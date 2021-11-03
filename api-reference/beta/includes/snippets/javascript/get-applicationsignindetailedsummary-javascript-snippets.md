---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9356f244d9e1636b3b24bbb801a74b02cf070d6dbb570805837dd1ae8187739c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898927"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let applicationSignInDetailedSummary = await client.api('/reports/applicationSignInDetailedSummary/{id}')
    .version('beta')
    .get();

```