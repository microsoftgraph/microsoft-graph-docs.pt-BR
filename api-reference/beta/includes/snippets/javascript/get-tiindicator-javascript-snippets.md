---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da21c1f2649247f24914723084ce95acd907284f9df4e794f91b0bc867fc69be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899622"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tiIndicator = await client.api('/security/tiIndicators/{id}')
    .version('beta')
    .get();

```