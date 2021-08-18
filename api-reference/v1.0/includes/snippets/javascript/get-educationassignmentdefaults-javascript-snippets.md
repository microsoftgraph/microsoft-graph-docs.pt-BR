---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e30c76dcd890d4fc14b14bfd209191703cfa41d7b3d9582f17edc3d06a195a1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103123"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationAssignmentDefaults = await client.api('/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentDefaults')
    .get();

```