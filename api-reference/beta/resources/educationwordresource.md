---
title: tipo de recurso de educationWordResource
description: 'Uma subclasse de educationResource. Esse é um recurso de documento do Word. O arquivo do Word deve ser carregado no diretório **fileResource** associado a '
ms.openlocfilehash: 28df3278a0d97f440014c342d592d2701b348d94
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038532"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="a8966-105">tipo de recurso de educationWordResource</span><span class="sxs-lookup"><span data-stu-id="a8966-105">educationWordResource resource type</span></span>

> <span data-ttu-id="a8966-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a8966-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8966-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a8966-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8966-108">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="a8966-108">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="a8966-109">Esse é um recurso de documento do Word.</span><span class="sxs-lookup"><span data-stu-id="a8966-109">This is a Word document resource.</span></span> <span data-ttu-id="a8966-110">O arquivo do Word deve ser carregado no diretório **fileResource** associado a atribuição ou o envio.</span><span class="sxs-lookup"><span data-stu-id="a8966-110">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="a8966-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8966-111">Properties</span></span>
| <span data-ttu-id="a8966-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8966-112">Property</span></span>     | <span data-ttu-id="a8966-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8966-113">Type</span></span>   |<span data-ttu-id="a8966-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8966-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8966-115">fileUrl</span><span class="sxs-lookup"><span data-stu-id="a8966-115">fileUrl</span></span>|<span data-ttu-id="a8966-116">String</span><span class="sxs-lookup"><span data-stu-id="a8966-116">String</span></span>|<span data-ttu-id="a8966-117">Local do arquivo no disco.</span><span class="sxs-lookup"><span data-stu-id="a8966-117">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8966-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8966-118">JSON representation</span></span>

<span data-ttu-id="a8966-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8966-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationWordResource"
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
  "description": "educationWordResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->