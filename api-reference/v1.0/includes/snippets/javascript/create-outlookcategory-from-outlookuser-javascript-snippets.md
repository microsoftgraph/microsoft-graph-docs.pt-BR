---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2448b93b6e1fea7590e42b062987cdb0c776ddde707a6375eda29294e879a9cc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272186"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookCategory = {
      displayName: 'Project expenses',
      color: 'preset9'
};

await client.api('/me/outlook/masterCategories')
    .post(outlookCategory);

```