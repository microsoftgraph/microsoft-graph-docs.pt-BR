---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8033f8b6803ebd674b8593428aa86e14e0a5cf2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444535"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/search(q='{search-query}')')
    .version('beta')
    .get();

```