---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e65ae3da5013a850cc80008598b8322b4184f1c94072be2f7423af01bf9abdd0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215135"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const removeMembersById = {
  ids: [
    'String',
    'String',
    'String'
  ],
  memberEntityType: '#microsoft.graph.windowsUpdates.azureADDevice'
};

await client.api('/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/removeMembersById')
    .version('beta')
    .post(removeMembersById);

```