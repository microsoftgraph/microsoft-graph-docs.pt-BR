---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9d53556ed95ab4e25803acbbfe3cb1830c4d18dad8bb534c387bd4a090cadd0e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898160"
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