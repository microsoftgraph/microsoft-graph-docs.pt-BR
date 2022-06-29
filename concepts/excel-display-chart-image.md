---
title: Exibir uma imagem de gráfico no Excel
description: Quando você recupera uma imagem de gráfico, a API do Excel no Microsoft Graph retorna a imagem como uma cadeia de caracteres de base 64 que você pode exibir dentro de uma marca de imagem HTML.
ms.localizationpriority: medium
author: lumine2008
ms.prod: excel
ms.openlocfilehash: ac1713d017ee982c4df5fc89ff4a28dc4437a4cf
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440850"
---
# <a name="display-a-chart-image-in-excel"></a>Exibir uma imagem de gráfico no Excel

Quando você executa uma [operação GET para](/graph/api/chart-image) recuperar uma imagem de gráfico, a API do Excel no Microsoft Graph retorna a imagem como uma cadeia de caracteres de base 64. Você pode exibir a cadeia de caracteres de base 64 dentro de uma marca de imagem HTML:

```html
 <img src="data:image/png;base64,{base-64 chart image string}/>
```

Para o comportamento padrão, use `Image(width=0,height=0,fittingMode='fit')`.

A seguir está um exemplo de uma imagem de gráfico retornada com os parâmetros padrão.

![A imagem de gráfico do Excel com altura e largura padrão.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

Se você quiser personalizar a exibição da imagem, especifique uma altura, largura e um modo de ajuste. Esta é a aparência da imagem de gráfico quando você a recupera com esses parâmetros: `Image(width=500,height=500,fittingMode='Fill')`.

## <a name="see-also"></a>Confira também

* [Gerenciar sessões do Excel usando o Microsoft Graph](excel-manage-sessions.md)
* [Gravar em uma pasta de trabalho do Excel usando o Microsoft Graph](excel-write-to-workbook.md)
* [Usar funções de pasta de trabalho do Excel com o Microsoft Graph](excel-use-functions.md)
* [Atualizar um formato de intervalo no Excel com o Microsoft Graph](excel-update-range-format.md)
* [Usar a API REST do Excel](/graph/api/resources/excel)
