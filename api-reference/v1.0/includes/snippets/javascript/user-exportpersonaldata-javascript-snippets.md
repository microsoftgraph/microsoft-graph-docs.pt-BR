---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 606f9dc35375ab7a2632d5b4970c9b093a980c13
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780592"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const exportPersonalData = {
  storageLocation: 'storageLocation-value'
};

await client.api('/users/{id}/exportPersonalData')
    .post(exportPersonalData);

```