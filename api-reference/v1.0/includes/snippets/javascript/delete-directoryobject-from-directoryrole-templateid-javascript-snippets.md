---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 871afcd0b9b3fa1e488c3af1188fc372ab57d7ea
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522791"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/roleTemplateId={role-templateId}/members/{user-id}/$ref')
    .delete();

```