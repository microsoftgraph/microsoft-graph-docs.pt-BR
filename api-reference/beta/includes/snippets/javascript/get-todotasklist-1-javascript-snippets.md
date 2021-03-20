---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e60fc327c077c0ed40c4109f813e136499d1bff5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953809"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let lists = await client.api('/me/todo/lists')
    .version('beta')
    .get();

```