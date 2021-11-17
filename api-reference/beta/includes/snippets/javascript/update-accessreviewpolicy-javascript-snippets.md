---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a781ff7fd05490a3569407caf05f7e2cdf17a8e218829c9a2d68d720edc4f691
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898152"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReviewPolicy = {
  isGroupOwnerManagementEnabled: true
};

await client.api('/policies/accessReviewPolicy')
    .version('beta')
    .update(accessReviewPolicy);

```