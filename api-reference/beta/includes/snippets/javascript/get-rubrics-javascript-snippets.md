---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5dbf209c8b249f02a1c6412f7834ba9153ab186
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461311"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/me/rubrics')
    .version('beta')
    .get();

```