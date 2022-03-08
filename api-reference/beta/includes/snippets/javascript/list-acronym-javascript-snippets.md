---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8f8b1dc547292633952269a8621230ac78a641a7
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338066"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let acronyms = await client.api('/search/acronyms')
    .version('beta')
    .get();

```