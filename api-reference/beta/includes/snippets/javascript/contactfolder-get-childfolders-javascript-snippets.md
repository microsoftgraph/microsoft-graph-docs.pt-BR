---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03040757a351c1532c340575100bb185a375dd1e988ee39ee944215457bab5be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273557"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let childFolders = await client.api('/me/contactFolders/{id}/childFolders')
    .version('beta')
    .get();

```