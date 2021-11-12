---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dc89bcbab15673a6f5c92ce909cd9a54b677aa5c2f79cb4cb4536d6841e1f768
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215557"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerTask = await client.api('/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh')
    .version('beta')
    .get();

```