---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f272e29012ad3a53918e9a12193b4112ff9851a4
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912916"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cancelMediaProcessingOperation = {
  clientContext: "clientContext-value"
};

let res = await client.api('/communications/calls/{id}/cancelMediaProcessing')
    .version('beta')
    .post(cancelMediaProcessingOperation);

```