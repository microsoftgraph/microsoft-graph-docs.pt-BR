---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6f8be0a1aa60ba6e10c0cc6157531af11f7c0c4d3a2f1a636494717faa7a5abe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159466"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plans = await client.api('/me/planner/plans')
    .get();

```