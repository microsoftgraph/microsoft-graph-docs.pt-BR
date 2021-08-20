---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb538f2f19f56f9472ce17ec184f75ce60dd4a531aa39c6efcabeaa4eee369b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100468"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationSubmission = await client.api('/education/classes/11010/assignments/19002/submissions/33223')
    .version('beta')
    .get();

```