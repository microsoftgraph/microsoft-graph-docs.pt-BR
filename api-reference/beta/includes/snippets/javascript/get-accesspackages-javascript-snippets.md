---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21bb1db44f662b49ec8326596fff703a2899eb4c
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994141"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/entitlementManagement/accessPackages')
    .version('beta')
    .get();

```