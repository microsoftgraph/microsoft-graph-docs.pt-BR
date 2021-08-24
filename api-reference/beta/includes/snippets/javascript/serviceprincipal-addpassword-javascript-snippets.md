---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b812faeaf256b9cac4c85c00bfdff61ffa81a95f622f95be0c606d745162503f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274722"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const addPassword = {
  passwordCredential: {
    displayName: 'Password friendly name'
  }
};

await client.api('/servicePrincipals/{id}/addPassword')
    .version('beta')
    .post(addPassword);

```