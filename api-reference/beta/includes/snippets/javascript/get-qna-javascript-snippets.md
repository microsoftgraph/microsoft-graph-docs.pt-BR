---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e19a83700d0b906bac5220a809688798e7d3281c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338008"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let qna = await client.api('/search/qnas/{qnaId}')
    .version('beta')
    .get();

```