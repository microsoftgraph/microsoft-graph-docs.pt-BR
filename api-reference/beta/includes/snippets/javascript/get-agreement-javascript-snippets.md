---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 87afddd3aca0a419b4e65d88227ff72d52be8aaf
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408494"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/agreements/{id}')
    .version('beta')
    .expand('files')
    .get();

```