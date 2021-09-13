---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0172825a288152182ab19e5defe5b897d38681653d6c12aff3a302f1ea988c71
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213952"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sections = await client.api('/me/onenote/notebooks/{id}/sections')
    .get();

```