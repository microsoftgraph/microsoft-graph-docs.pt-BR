---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0878bbadabf30b14f8125f028ad5afc210f04b1008811d740bc79120ce5bdf80
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216432"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let oauth2PermissionGrants = await client.api('/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/oauth2PermissionGrants')
    .get();

```