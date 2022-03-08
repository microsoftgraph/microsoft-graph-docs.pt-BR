---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 830f17a211ce46ff3c81000512fce59f0f157411
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338056"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookmark = await client.api('/search/bookmarks/{bookmarksId}')
    .version('beta')
    .get();

```