---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1cca2c49cbc3978d3f0709715f3f850dc8352a72e6f3db07db5916d2cc4e6f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216334"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rooms = await client.api('/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms')
    .version('beta')
    .get();

```