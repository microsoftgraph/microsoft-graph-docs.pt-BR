---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 768f0444780ee0a15d2fdc37a312c7a45382226d766cfbf1ca1e33976ef3db8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099505"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{id}/delegatedPermissionClassifications/{id}')
    .version('beta')
    .delete();

```