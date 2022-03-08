---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 40c7b2d33327fa148a1316196e396d17ec2f593f
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337567"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/accessReviews/historyDefinitions/b2cb022f-b7e1-40f3-9854-c65a40861c38/instances/b2cb022f-b7e1-40f3-9854-c65a40861c38/generateDownloadUri')
    .post();

```