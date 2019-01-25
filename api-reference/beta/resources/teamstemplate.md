---
title: tipo de recurso de teamsTemplate
description: Descreve a entidade teamsTemplate.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e75b3d8df318b116d5d908a40d4f756d9ee70864
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513043"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="32842-103">tipo de recurso de teamsTemplate</span><span class="sxs-lookup"><span data-stu-id="32842-103">teamsTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32842-104">Um modelo de equipe é um blueprint para a criação de uma [equipe](../resources/team.md) no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="32842-104">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="32842-105">Um modelo especifica a estrutura, configurações e até mesmo conteúdo que deve ser provisionado em uma nova criada usando o modelo de equipe.</span><span class="sxs-lookup"><span data-stu-id="32842-105">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="32842-106">A Microsoft fornece um pacote de modelos de base e os clientes podem salvar seus próprios modelos personalizados.</span><span class="sxs-lookup"><span data-stu-id="32842-106">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="32842-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32842-107">Properties</span></span>

| <span data-ttu-id="32842-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32842-108">Property</span></span>            | <span data-ttu-id="32842-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="32842-109">Type</span></span>     | <span data-ttu-id="32842-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="32842-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="32842-111">id</span><span class="sxs-lookup"><span data-stu-id="32842-111">id</span></span>                  | <span data-ttu-id="32842-112">String</span><span class="sxs-lookup"><span data-stu-id="32842-112">String</span></span>   | <span data-ttu-id="32842-113">Identificador exclusivo do modelo.</span><span class="sxs-lookup"><span data-stu-id="32842-113">Unique identifier of the template.</span></span> <span data-ttu-id="32842-114">Não pode ser nula.</span><span class="sxs-lookup"><span data-stu-id="32842-114">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="32842-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32842-115">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTemplate",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

# <a name="see-also"></a><span data-ttu-id="32842-116">Confira também</span><span class="sxs-lookup"><span data-stu-id="32842-116">See also</span></span>

- [<span data-ttu-id="32842-117">equipe</span><span class="sxs-lookup"><span data-stu-id="32842-117">team</span></span>](team.md)

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
