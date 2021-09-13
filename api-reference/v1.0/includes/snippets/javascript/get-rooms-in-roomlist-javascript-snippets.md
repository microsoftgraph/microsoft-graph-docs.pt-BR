---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9185f0bf13ee114a82820566de46f2633e97ceccfc3c100cdb04a40285c1a0d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272002"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rooms = await client.api('/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms')
    .get();

```