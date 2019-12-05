---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d77bb3c77552f00e31c39d747791a05d2489a7a0
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37997034"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const place = {
  @odata.type: "microsoft.graph.roomlist",
  displayName: "Building 1",
  phone:"555-555-0100"
};

let res = await client.api('/places/Building1RroomList@contoso.onmicrosoft.com')
    .version('beta')
    .update(place);

```