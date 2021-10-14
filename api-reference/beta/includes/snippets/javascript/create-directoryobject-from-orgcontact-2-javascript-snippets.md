---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c88b48f4162f71bd3a169f6f204a77c47a40e597361917d99f8f00e6edba0ecf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159657"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  directoryObject: {
  }
};

await client.api('/contacts/{id}/memberOf')
    .version('beta')
    .post(directoryObject);

```