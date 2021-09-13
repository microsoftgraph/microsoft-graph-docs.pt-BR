---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c450746c20332a3831a8a4d0c4a3ef2b9574a090ef1bec4af784e9d1889767f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157330"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFormat = {
  columnWidth: 135,
  verticalAlignment: 'Top',
  rowHeight: 49,
  wrapText: false
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$A$1')/format')
    .update(workbookRangeFormat);

```