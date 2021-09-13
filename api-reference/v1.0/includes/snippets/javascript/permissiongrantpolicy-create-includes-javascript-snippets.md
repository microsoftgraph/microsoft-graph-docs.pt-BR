---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7016f1679e7a02f88eca78a67e5b4cba617679832251b810e2f75b01795f1a4f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099302"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permissionGrantConditionSet = {
  permissionType: 'delegated',
  clientApplicationsFromVerifiedPublisherOnly: true
};

await client.api('/policies/permissionGrantPolicies/{id}/includes')
    .post(permissionGrantConditionSet);

```