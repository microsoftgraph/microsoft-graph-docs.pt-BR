---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4c4f05ed408387e4e2471ad5d03863018de787e97d05072608cc705418c33f5d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326681"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookWorksheetProtection = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/protection')
    .get();

```