---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 885f4f1ce713e8159058b970f5b417ca2780f546
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338421"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/search/qnas/{qnaId}')
    .version('beta')
    .delete();

```