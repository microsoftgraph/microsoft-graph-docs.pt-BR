---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 80eee941cee1f4d762a0a0bebe16844bd8f80e2e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37402416"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .version('beta')
    .filter('identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')')
    .select('displayName,id')
    .get();

```