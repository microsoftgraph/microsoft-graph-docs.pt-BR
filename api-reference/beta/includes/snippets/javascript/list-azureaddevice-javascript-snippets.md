---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 994045da6c00d65b0fa7dba6fd4d126ed49b6a3d59a5c3aef5eb82ecf0ff41ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329526"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let updatableAssets = await client.api('/admin/windows/updates/updatableAssets/')
    .version('beta')
    .filter('isof(\'microsoft.graph.windowsUpdates.azureADDevice\')')
    .get();

```