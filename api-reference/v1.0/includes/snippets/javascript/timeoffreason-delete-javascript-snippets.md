---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2c20d987732c8c40dfae6901caf2fd340c585b14096377c097cd4e1bac27d4c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217221"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}')
    .delete();

```