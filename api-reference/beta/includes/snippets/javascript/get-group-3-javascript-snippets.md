---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7c6403100dd3960a73f5df34c90dad075eafe4048a2553eccda9d186105faa6b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327296"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/termStore/groups/1FFD3F87-9464-488A-A0EC-8FB90911182C')
    .version('beta')
    .get();

```