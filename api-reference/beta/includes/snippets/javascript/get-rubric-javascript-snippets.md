---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f523daa090fe99ad546b78ea78e77bd97de1c81c
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461187"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/me/assignments/{id}/rubric')
    .version('beta')
    .get();

```