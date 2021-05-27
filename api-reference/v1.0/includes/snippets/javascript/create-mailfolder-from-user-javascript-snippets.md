---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb77572c342b8d85c914b7d3b6c291941c5fbf41
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668569"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: 'Clutter',
  isHidden: true
};

await client.api('/me/mailFolders')
    .post(mailFolder);

```