---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dda41d3950e069957dcbf177bbb6df18250f2764
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338076"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const acronym = {
  description: 'A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers.'
};

await client.api('/search/acronyms/{acronymsId}')
    .version('beta')
    .update(acronym);

```