---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ebf593d54212e21931a8b32686d3bdd9ea885051e125e2244fc4882293dcb19e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160075"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let outlookTaskFolder = await client.api('/me/outlook/taskFolders/AAMkADIyAAAAABrJAAA=')
    .version('beta')
    .get();

```