---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe881577b8b52ea59899e59437e93daf43478502
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806650"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/delta')
    .get();

```