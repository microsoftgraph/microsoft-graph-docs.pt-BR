---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e5130a72cb08c2ec58af008eb77f37cf0489ebc3cc0a462082bd491f3fe33be0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272930"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let callRecord = await client.api('/communications/callRecords/{id}')
    .expand('sessions($expand=segments)')
    .get();

```