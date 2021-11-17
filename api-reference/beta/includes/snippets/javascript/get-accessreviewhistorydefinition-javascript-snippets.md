---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3e51e5439cf8460ffaec8900fe6a719f2c6f6041a3aee812755477ceae0c610
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898215"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReviewHistoryDefinition = await client.api('/identityGovernance/accessReviews/historyDefinitions/b2cb022f-b7e1-40f3-9854-c65a40861c38')
    .version('beta')
    .get();

```