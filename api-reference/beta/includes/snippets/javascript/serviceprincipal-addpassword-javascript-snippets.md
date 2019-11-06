---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a8484d8e531a68c05a1e95e32606554db1b6f2fa
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997656"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const addPassword = {
  passwordCredential: {
    displayName: "Password friendly name"
  }
};

let res = await client.api('/servicePrincipals/{id}/addPassword')
    .version('beta')
    .post(addPassword);

```