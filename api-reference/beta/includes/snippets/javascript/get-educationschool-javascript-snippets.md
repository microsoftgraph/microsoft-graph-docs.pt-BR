---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8ad9148d039b26f0a69d72f8539210ea16acc862008f25ebfbb8bdc8fb114064
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159222"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationSchool = await client.api('/education/schools/10001')
    .version('beta')
    .get();

```