---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 161abcc7a986141f0670c2e279f74cf45500b7fdcbeb0555144fc84e88aefa49
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156592"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageCatalogs = await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs')
    .version('beta')
    .get();

```