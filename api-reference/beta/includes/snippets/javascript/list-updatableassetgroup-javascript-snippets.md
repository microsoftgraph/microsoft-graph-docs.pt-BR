---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cada82132ab420b25e6bcbd6a86c5f3f889d3ca7
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239248"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let updatableAssets = await client.api('/admin/windows/updates/updatableAssets/')
    .version('beta')
    .filter('isof(\'microsoft.graph.windowsUpdates.updatableAssetGroup\')')
    .get();

```