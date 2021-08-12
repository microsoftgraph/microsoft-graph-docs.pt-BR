---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 908e53372aba156191850c5d5f1ef034ceda0bc809b0082db7b402bbfd9355e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237697"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFont workbookRangeFont = new WorkbookRangeFont();
workbookRangeFont.italic = true;
workbookRangeFont.size = 26;

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range("$B$1").format().font()
    .buildRequest()
    .patch(workbookRangeFont);

```