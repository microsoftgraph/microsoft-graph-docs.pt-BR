---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c5f7cf1d116e051522175070cc9679ad90ba9321
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240617"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReviewPolicy = {
  isGroupOwnerManagementEnabled: true
};

await client.api('/identityGovernance/accessReviews/policy')
    .version('beta')
    .update(accessReviewPolicy);

```