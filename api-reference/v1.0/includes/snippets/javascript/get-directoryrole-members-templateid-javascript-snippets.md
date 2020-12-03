---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 11353818631c15e1313e26996087bab97abf84fe
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524551"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf/members')
    .get();

```