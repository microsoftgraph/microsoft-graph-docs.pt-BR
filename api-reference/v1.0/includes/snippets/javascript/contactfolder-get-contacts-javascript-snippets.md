---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 51aae316c9626deb607f52f7bde6b6ea460d461a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883875"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contactFolders/{id}/contacts')
    .get();

```