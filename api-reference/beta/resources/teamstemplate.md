---
title: tipo de recurso Teams
description: Descreve a entidade Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e75b3d8df318b116d5d908a40d4f756d9ee70864
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583162"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="74af0-103">tipo de recurso Teams</span><span class="sxs-lookup"><span data-stu-id="74af0-103">teamsTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74af0-104">Um modelo de equipe é um gráfico para a criação de uma [equipe](../resources/team.md) no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="74af0-104">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="74af0-105">Um modelo especifica a estrutura, as configurações e até o conteúdo que deve ser provisionado em uma nova equipe criada usando o modelo.</span><span class="sxs-lookup"><span data-stu-id="74af0-105">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="74af0-106">A Microsoft fornece um pacote de modelos básicos e os clientes podem salvar seus próprios modelos personalizados.</span><span class="sxs-lookup"><span data-stu-id="74af0-106">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="74af0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74af0-107">Properties</span></span>

| <span data-ttu-id="74af0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74af0-108">Property</span></span>            | <span data-ttu-id="74af0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="74af0-109">Type</span></span>     | <span data-ttu-id="74af0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="74af0-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="74af0-111">id</span><span class="sxs-lookup"><span data-stu-id="74af0-111">id</span></span>                  | <span data-ttu-id="74af0-112">String</span><span class="sxs-lookup"><span data-stu-id="74af0-112">String</span></span>   | <span data-ttu-id="74af0-113">Identificador exclusivo do modelo.</span><span class="sxs-lookup"><span data-stu-id="74af0-113">Unique identifier of the template.</span></span> <span data-ttu-id="74af0-114">Não pode ser nulo.</span><span class="sxs-lookup"><span data-stu-id="74af0-114">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="74af0-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74af0-115">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="74af0-116">Confira também</span><span class="sxs-lookup"><span data-stu-id="74af0-116">See also</span></span>

- [<span data-ttu-id="74af0-117">team</span><span class="sxs-lookup"><span data-stu-id="74af0-117">team</span></span>](team.md)

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
