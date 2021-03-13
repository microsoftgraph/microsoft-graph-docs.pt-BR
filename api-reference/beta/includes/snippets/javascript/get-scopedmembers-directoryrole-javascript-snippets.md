---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb95e1d31cc1fb22ed201a1935338964cbc231a4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789710"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let scopedMembers = await client.api('/directoryRoles/{id}/scopedMembers')
    .version('beta')
    .get();

```