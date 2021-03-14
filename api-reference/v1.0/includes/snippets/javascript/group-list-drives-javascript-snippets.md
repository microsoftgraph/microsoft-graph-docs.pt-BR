---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dfc8d434a06383e92a36b72a4b5481fcdf819944
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810388"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drives = await client.api('/groups/{groupId}/drives')
    .get();

```