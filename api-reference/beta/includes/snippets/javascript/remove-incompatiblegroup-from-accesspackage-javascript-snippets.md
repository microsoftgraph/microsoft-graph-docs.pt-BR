---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6328360e9b5c5e986496c8f0931245e88715a4bc89ffcd1e0dc307ff08d97325
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156624"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups/{id}/$ref')
    .version('beta')
    .delete();

```