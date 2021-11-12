---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: edc33387f50486e6f844bde72943b65ec5f4fcb8d3471c3d6693a55119c90e5a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272367"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contactFolder = await client.api('/me/contactFolders/{id}')
    .version('beta')
    .get();

```