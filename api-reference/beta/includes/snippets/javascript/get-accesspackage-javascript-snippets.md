---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59f97fb39993ccd0bd7c4cacfb9b1ffb3c04d632a6c9ec308b891880b0c30f8e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898822"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackage = await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}')
    .version('beta')
    .get();

```