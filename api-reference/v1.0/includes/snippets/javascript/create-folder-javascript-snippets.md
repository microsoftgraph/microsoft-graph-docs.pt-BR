---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2366f2d85b7599674ab80777a643e5bfe4d414c808f8a4fabd1bbb546b00d6d3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57406767"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: 'New Folder',
  folder: { },
  '@microsoft.graph.conflictBehavior': 'rename'
};

await client.api('/me/drive/root/children')
    .post(driveItem);

```