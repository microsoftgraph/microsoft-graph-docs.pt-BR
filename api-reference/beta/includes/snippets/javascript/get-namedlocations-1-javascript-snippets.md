---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 67be56ffe9e77631f1f22c2ad7d7b1a8ceef253fa1350198d2cbe1f3fe8d60d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159700"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let namedLocations = await client.api('/identity/conditionalAccess/namedLocations')
    .version('beta')
    .get();

```