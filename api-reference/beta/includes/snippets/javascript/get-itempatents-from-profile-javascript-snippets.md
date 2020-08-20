---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24e0c1913c2025c16333b4e03fb6af2bf75450ce
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820134"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/patents')
    .version('beta')
    .get();

```