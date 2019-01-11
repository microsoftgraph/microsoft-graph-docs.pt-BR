---
title: tipo de recurso de educationPowerPointResource
description: 'Uma subclasse de educationResource. Esse é um recurso do PowerPoint. O arquivo do PowerPoint que deve ser carregado no diretório **fileResource** associado a '
localization_priority: Normal
ms.openlocfilehash: 763a529e97b12c93d8f10aa6855c20818c02da67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845455"
---
# <a name="educationpowerpointresource-resource-type"></a><span data-ttu-id="359dd-105">tipo de recurso de educationPowerPointResource</span><span class="sxs-lookup"><span data-stu-id="359dd-105">educationPowerPointResource resource type</span></span>

> <span data-ttu-id="359dd-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="359dd-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="359dd-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="359dd-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="359dd-108">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="359dd-108">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="359dd-109">Esse é um recurso do PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="359dd-109">This is a PowerPoint resource.</span></span> <span data-ttu-id="359dd-110">O arquivo do PowerPoint deve ser carregado no diretório **fileResource** associado a atribuição ou o envio.</span><span class="sxs-lookup"><span data-stu-id="359dd-110">The PowerPoint file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="359dd-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="359dd-111">Properties</span></span>
| <span data-ttu-id="359dd-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="359dd-112">Property</span></span>     | <span data-ttu-id="359dd-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="359dd-113">Type</span></span>   |<span data-ttu-id="359dd-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="359dd-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="359dd-115">fileUrl</span><span class="sxs-lookup"><span data-stu-id="359dd-115">fileUrl</span></span>|<span data-ttu-id="359dd-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="359dd-116">String</span></span>|<span data-ttu-id="359dd-117">Local do arquivo no disco.</span><span class="sxs-lookup"><span data-stu-id="359dd-117">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="359dd-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="359dd-118">JSON representation</span></span>

<span data-ttu-id="359dd-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="359dd-119">The following is a JSON representation of the resource.</span></span>

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
