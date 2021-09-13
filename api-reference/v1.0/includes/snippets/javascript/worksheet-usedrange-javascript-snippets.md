---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d4a98787a24b8846e68a453704904c7729bca4d52b04f7b39b144cde05c65caa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271874"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange')
    .get();

```