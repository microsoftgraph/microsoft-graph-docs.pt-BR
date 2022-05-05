---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0a8fa981b62641c701acc898afdaf7e3d9eb10f
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203829"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let incompatibleAccessPackages = await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages')
    .version('beta')
    .get();

```