---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe8281b2e806b4c35730cf5a6e1e590e104eb0f9ea1421b5d3e708beeb2764bb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100434"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerBucketTaskBoardTaskFormat = await client.api('/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/bucketTaskBoardFormat')
    .version('beta')
    .get();

```