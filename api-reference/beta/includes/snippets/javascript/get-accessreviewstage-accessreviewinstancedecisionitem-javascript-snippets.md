---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 665c99c62378e359eae0448765fb93df20fad61e
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/16/2022
ms.locfileid: "62853248"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReviewInstanceDecisionItem = await client.api('/identityGovernance/accessReviews/definitions/5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0/instances/6444d4fd-ab55-4608-8cf9-c6702d172bcc/stages/9458f255-dff2-4d86-9a05-69438f49d7f8/decisions/e6cafba0-cbf0-4748-8868-0810c7f4cc06')
    .version('beta')
    .get();

```