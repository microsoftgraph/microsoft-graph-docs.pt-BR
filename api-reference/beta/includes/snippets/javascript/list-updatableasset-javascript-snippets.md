---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0fe7296371d94ea0d574315326939d3ca8a78b86
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "61004286"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/microsoft.graph.windowsUpdates.updatableAssetGroup/members')
    .version('beta')
    .get();

```