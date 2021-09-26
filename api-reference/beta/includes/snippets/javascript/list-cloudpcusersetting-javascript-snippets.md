---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af72729b50b87815414199b55b594f507fc2d9caf24460bbe4d4fc86b7f22ace
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157172"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userSettings = await client.api('/deviceManagement/virtualEndpoint/userSettings')
    .version('beta')
    .get();

```