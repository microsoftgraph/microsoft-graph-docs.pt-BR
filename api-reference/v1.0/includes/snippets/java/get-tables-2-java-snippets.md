---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2da46f439cda2788f199b6ec3ad0900a9d57feb
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209348"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookNamedItemCollectionPage names = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").names()
    .buildRequest()
    .get();

```