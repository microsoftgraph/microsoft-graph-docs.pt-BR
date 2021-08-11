---
title: Exibir uma imagem de gráfico do Excel com o Microsoft Graph
description: Ao executar uma operação GET para recuperar uma imagem de gráfico, a API do Excel retorna a imagem como uma cadeia de caracteres de Base 64.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 6e456a8008eb3d50da818c2e3da1a48ca54f4211eb5b1e8300dd3bef6dbf5e59
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54149566"
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
