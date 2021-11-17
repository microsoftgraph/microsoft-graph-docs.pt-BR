---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fcc384e69fe385edbe6047ea7ea06aa53158bfc285ab973fb63ec451c9e44847
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273377"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let policies = await client.api('/identity/conditionalAccess/policies')
    .version('beta')
    .filter('displayName eq \'SimplePolicy1\' or displayName eq \'SimplePolicy2\'')
    .get();

```