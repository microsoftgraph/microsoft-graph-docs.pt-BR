---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e6bea515a1d50d661f723763a22af026b29cdc79651e4644e864d6ada60f60c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214399"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/me/messages/4aade2547798441eab5188a7a2436bc1/$value')
    .get();

```