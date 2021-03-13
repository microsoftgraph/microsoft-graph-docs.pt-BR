---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c897de6e9c2e8e659445cfb5c503fb7e6c0d118d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804545"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contactFolder = {
  displayName: 'displayName-value'
};

await client.api('/me/contactFolders/{id}/childFolders')
    .version('beta')
    .post(contactFolder);

```