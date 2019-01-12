---
title: tipo de recurso de educationPowerPointResource
description: 'Uma subclasse de educationResource. Esse é um recurso do PowerPoint. O arquivo do PowerPoint que deve ser carregado no diretório **fileResource** associado a '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: f92d74d8e3dfb7cebcecd607bbd4bd8e2f3b43da
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940663"
---
# <a name="educationpowerpointresource-resource-type"></a><span data-ttu-id="89299-105">tipo de recurso de educationPowerPointResource</span><span class="sxs-lookup"><span data-stu-id="89299-105">educationPowerPointResource resource type</span></span>

> <span data-ttu-id="89299-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="89299-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89299-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="89299-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="89299-108">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="89299-108">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="89299-109">Esse é um recurso do PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="89299-109">This is a PowerPoint resource.</span></span> <span data-ttu-id="89299-110">O arquivo do PowerPoint deve ser carregado no diretório **fileResource** associado a atribuição ou o envio.</span><span class="sxs-lookup"><span data-stu-id="89299-110">The PowerPoint file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="89299-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89299-111">Properties</span></span>
| <span data-ttu-id="89299-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89299-112">Property</span></span>     | <span data-ttu-id="89299-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="89299-113">Type</span></span>   |<span data-ttu-id="89299-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="89299-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89299-115">fileUrl</span><span class="sxs-lookup"><span data-stu-id="89299-115">fileUrl</span></span>|<span data-ttu-id="89299-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89299-116">String</span></span>|<span data-ttu-id="89299-117">Local do arquivo no disco.</span><span class="sxs-lookup"><span data-stu-id="89299-117">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89299-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89299-118">JSON representation</span></span>

<span data-ttu-id="89299-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="89299-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerPointResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationPowerPointResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
