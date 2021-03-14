---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf1dbc487d0bf0689348cc86acc8ed0cf3bd87ca
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793256"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryRole = {
  roleTemplateId: 'roleTemplateId-value'
};

await client.api('/directoryRoles')
    .post(directoryRole);

```