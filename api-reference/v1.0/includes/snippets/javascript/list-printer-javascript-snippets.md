---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38d75d76d2352a36b305b4293b09fefbed735d1b3ae1e499a0c4721096fff55e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156383"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printers = await client.api('/print/printers')
    .get();

```