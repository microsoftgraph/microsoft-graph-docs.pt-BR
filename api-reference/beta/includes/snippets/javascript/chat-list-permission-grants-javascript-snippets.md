---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b7bc11161a279a358de3a9b45cd0d882b295968fd0cd2a889932c7b4fda4b976
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900247"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permissionGrants = await client.api('/chats/19:089ac694c48647c68035aae675cf78ab@thread.v2/permissionGrants')
    .version('beta')
    .get();

```