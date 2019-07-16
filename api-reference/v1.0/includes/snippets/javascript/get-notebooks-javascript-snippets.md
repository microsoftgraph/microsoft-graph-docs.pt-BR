---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 628ad7fe31632c0ddae3959b1a2101b59bd57ebc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737410"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/notebooks')
    .get();

```