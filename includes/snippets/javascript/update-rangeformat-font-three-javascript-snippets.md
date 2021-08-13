---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c72d087e955d9b98e51a42e08022b7b0145c015507f243adcd1b996b15102523
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237727"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  underline: "Single",
  color: "#FFFFFF",
  size: 26
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/font')
    .update(workbookRangeFont);

```