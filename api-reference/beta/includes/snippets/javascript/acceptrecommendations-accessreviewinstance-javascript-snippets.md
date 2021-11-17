---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bdf353b14962391857018ecc0ef9b6a6a51faf9ba6755f1955511fab61da8178
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898209"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/acceptRecommendations')
    .version('beta')
    .post();

```