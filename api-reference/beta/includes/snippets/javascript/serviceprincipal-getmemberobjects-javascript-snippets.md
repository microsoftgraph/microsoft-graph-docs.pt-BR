---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f85dc129f6bec87bdb77a7b41a89c05a59c156c4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717822"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  securityEnabledOnly: true
};

let res = await client.api('/servicePrincipals/{id}/getMemberObjects')
    .version('beta')
    .post(String);

```