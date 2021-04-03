---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8246c44268f8ffeed81f4cc3ff9e69f2e0d76a05
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508796"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let oauth2PermissionGrants = await client.api('/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/oauth2PermissionGrants')
    .version('beta')
    .get();

```