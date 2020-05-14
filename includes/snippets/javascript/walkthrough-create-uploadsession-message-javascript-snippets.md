---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: efcb757d5e0a77ef77a70708a30421ae7e48af9f
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44052415"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const uploadSession = {
  AttachmentItem: {
    attachmentType: "file",
    name: "flower",
    size: 3483322
  }
};

let res = await client.api('/me/messages/AAMkADI5MAAIT3drCAAA=/attachments/createUploadSession')
    .version('beta')
    .post(uploadSession);

```