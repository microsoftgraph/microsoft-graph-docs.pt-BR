---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 215d2fbfc4d925a7c1bef716a4ae640ba02bc75453c2ebf44006fd9d4163e91c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237723"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  bold: true,
  color: "#4B180E",
  size: 26
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/font')
    .update(workbookRangeFont);

```