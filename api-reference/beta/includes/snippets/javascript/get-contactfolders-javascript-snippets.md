---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2e1b92c0a28e37c23f5dbd96da2b0ab31c5f8e75b77a33e8e5113533271a43f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899990"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contactFolders = await client.api('/me/contactFolders')
    .version('beta')
    .get();

```