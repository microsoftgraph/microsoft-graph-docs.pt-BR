---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1ad4a919a24da5fdca08f811707cb39e001e994f1ea364c5941f9584cd7e8a21
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329242"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unenrollAssetsById = {
  updateCategory: 'feature',
  memberEntityType: '#microsoft.graph.windowsUpdates.azureADDevice',
  ids: [
    'String',
    'String',
    'String'
  ]
};

await client.api('/admin/windows/updates/updatableAssets/unenrollAssetsById')
    .version('beta')
    .post(unenrollAssetsById);

```