---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6aadcdfc0c43a00b705d4a160a4cddab7271f2f5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892749"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/notebooks/{id}/sectionGroups')
    .get();

```