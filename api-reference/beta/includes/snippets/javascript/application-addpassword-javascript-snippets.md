---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c77ebc526cee9f245efe2c55258a76f33914dce2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794284"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const passwordCredential = {
  passwordCredential: {
    displayName: 'Password friendly name'
  }
};

await client.api('/applications/{id}/addPassword')
    .version('beta')
    .post(passwordCredential);

```