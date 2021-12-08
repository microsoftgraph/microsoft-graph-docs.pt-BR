---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da6b4009235055be2540b89974a53a6dac606f3d
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61347269"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}')
    .delete();

```