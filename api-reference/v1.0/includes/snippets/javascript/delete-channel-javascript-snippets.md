---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85d51238d0191aae04a43d2a247a5311e5daad209dd21e69406374ba5083e134
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57406907"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{id}/channels/{id}')
    .delete();

```