---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c80dbf0c9d263ab3b8e55adae3d073c6ca694ada
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089253"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/roleManagement/cloudPc/roleDefinitions/b7f5ddc1-b7dc-4d37-abce-b9d6fc15ffff')
    .version('beta')
    .delete();

```