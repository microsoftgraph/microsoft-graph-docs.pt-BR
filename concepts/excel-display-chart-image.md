---
title: Exibir uma imagem de gráfico do Excel com o Microsoft Graph
description: Ao executar uma operação GET para recuperar uma imagem de gráfico, a API do Excel retorna a imagem como uma cadeia de caracteres de Base 64.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 5cdf5522ccd0a72798ee62211e9221cf2ea9cd53
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946368"
---
# <a name="display-a-chart-image-in-excel-with-microsoft-graph"></a><span data-ttu-id="f9cc2-103">Exibir uma imagem de gráfico do Excel com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f9cc2-103">Display a chart image in Excel with Microsoft Graph</span></span>

<span data-ttu-id="f9cc2-104">Ao executar uma [operação GET para recuperar uma imagem de gráfico](/api-reference/v1.0/api/chart-image.md), a API do Excel retorna a imagem como uma cadeia de caracteres de Base 64.</span><span class="sxs-lookup"><span data-stu-id="f9cc2-104">When you perform a [GET operation to retrieve a chart image](/api-reference/v1.0/api/chart-image.md), the Excel API returns the image as a base-64 string.</span></span>

<span data-ttu-id="f9cc2-105">Você pode exibir a cadeia de caracteres de Base 64 dentro de uma marca de imagem HTML: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="f9cc2-105">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="f9cc2-106">Para o comportamento padrão, use `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="f9cc2-106">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="f9cc2-107">Veja um exemplo de uma imagem de gráfico retornada com os parâmetros padrão.</span><span class="sxs-lookup"><span data-stu-id="f9cc2-107">Here is an example of a chart image returned with the default parameters.</span></span>

![A imagem de gráfico do Excel com altura e largura padrão.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="f9cc2-109">Se você quiser personalizar a exibição da imagem, especifique uma altura, largura e um modo de ajuste.</span><span class="sxs-lookup"><span data-stu-id="f9cc2-109">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="f9cc2-110">Esta é a aparência da imagem de gráfico quando você a recupera com esses parâmetros: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="f9cc2-110">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

## <a name="see-also"></a><span data-ttu-id="f9cc2-111">Confira também</span><span class="sxs-lookup"><span data-stu-id="f9cc2-111">See also</span></span>

* [<span data-ttu-id="f9cc2-112">Gerenciar sessões do Excel usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f9cc2-112">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="f9cc2-113">Gravar em uma pasta de trabalho do Excel usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f9cc2-113">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="f9cc2-114">Usar funções de pasta de trabalho do Excel com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f9cc2-114">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="f9cc2-115">Atualizar um formato de intervalo no Excel com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f9cc2-115">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="f9cc2-116">Usar a API REST do Excel</span><span class="sxs-lookup"><span data-stu-id="f9cc2-116">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
