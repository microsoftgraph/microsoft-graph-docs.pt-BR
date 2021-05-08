---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a65a95253d9f516b6d09655db0d48a73fc8ee3a3
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239481"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const addMembersById = {
  ids: [
    'String',
    'String',
    'String'
  ],
  memberEntityType: '#microsoft.graph.windowsUpdates.azureADDevice'
};

await client.api('/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/addMembersById')
    .version('beta')
    .post(addMembersById);

```