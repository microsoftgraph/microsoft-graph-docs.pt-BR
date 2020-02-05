---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6751e6c51665993eb0c7f55bedab71857c1c173a
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774500"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/{class-id}/members')
    .get();

```