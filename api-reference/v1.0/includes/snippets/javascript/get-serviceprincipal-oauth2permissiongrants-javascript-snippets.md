---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b2060065d57ef0ff7c4a4a4bee24069e1866d19fbaa5bf6841baf0d39677fdc2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275299"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let oauth2PermissionGrants = await client.api('/servicePrincipals/{id}/oauth2PermissionGrants')
    .get();

```