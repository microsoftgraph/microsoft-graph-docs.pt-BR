---
title: Exibir uma imagem de gráfico do Excel com o Microsoft Graph
description: Ao executar uma operação GET para recuperar uma imagem de gráfico, a API do Excel retorna a imagem como uma cadeia de caracteres de Base 64.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 330c7d3a531a5735e824dda61928c3af2f05e5e3
ms.sourcegitcommit: ca55fc5f5711966eaa41da31cd1ae99820e9e586
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2019
ms.locfileid: "35645209"
---
# <a name="display-a-chart-image-in-excel-with-microsoft-graph"></a>Exibir uma imagem de gráfico do Excel com o Microsoft Graph

Ao executar uma [operação GET para recuperar uma imagem de gráfico](/graph/api/chart-image?view=graph-rest-1.0), a API do Excel retorna a imagem como uma cadeia de caracteres de Base 64.

Você pode exibir a cadeia de caracteres de Base 64 dentro de uma marca de imagem HTML: `<img src="data:image/png;base64,{base-64 chart image string}/>`.

Para o comportamento padrão, use `Image(width=0,height=0,fittingMode='fit')`. Veja um exemplo de uma imagem de gráfico retornada com os parâmetros padrão.

![A imagem de gráfico do Excel com altura e largura padrão.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

Se você quiser personalizar a exibição da imagem, especifique uma altura, largura e um modo de ajuste. Esta é a aparência da imagem de gráfico quando você a recupera com esses parâmetros: `Image(width=500,height=500,fittingMode='Fill')`.

## <a name="see-also"></a>Confira também

* [Gerenciar sessões do Excel usando o Microsoft Graph](excel-manage-sessions.md)
* [Gravar em uma pasta de trabalho do Excel usando o Microsoft Graph](excel-write-to-workbook.md)
* [Usar funções de pasta de trabalho do Excel com o Microsoft Graph](excel-use-functions.md)
* [Atualizar um formato de intervalo no Excel com o Microsoft Graph](excel-update-range-format.md)
* [Usar a API REST do Excel](/graph/api/resources/excel?view=graph-rest-1.0)
