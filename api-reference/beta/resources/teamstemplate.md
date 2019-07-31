---
title: tipo de recurso Teams
description: Descreve a entidade Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dde08e6c4ecde3b3a600958a5af5cd93b5fc600f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964386"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="f5638-103">tipo de recurso Teams</span><span class="sxs-lookup"><span data-stu-id="f5638-103">teamsTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5638-104">Um modelo de equipe é um gráfico para a criação de uma [equipe](../resources/team.md) no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f5638-104">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="f5638-105">Um modelo especifica a estrutura, as configurações e até o conteúdo que deve ser provisionado em uma nova equipe criada usando o modelo.</span><span class="sxs-lookup"><span data-stu-id="f5638-105">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="f5638-106">A Microsoft fornece um pacote de modelos básicos e os clientes podem salvar seus próprios modelos personalizados.</span><span class="sxs-lookup"><span data-stu-id="f5638-106">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="f5638-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5638-107">Properties</span></span>

| <span data-ttu-id="f5638-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5638-108">Property</span></span>            | <span data-ttu-id="f5638-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5638-109">Type</span></span>     | <span data-ttu-id="f5638-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5638-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="f5638-111">id</span><span class="sxs-lookup"><span data-stu-id="f5638-111">id</span></span>                  | <span data-ttu-id="f5638-112">String</span><span class="sxs-lookup"><span data-stu-id="f5638-112">String</span></span>   | <span data-ttu-id="f5638-113">Identificador exclusivo do modelo.</span><span class="sxs-lookup"><span data-stu-id="f5638-113">Unique identifier of the template.</span></span> <span data-ttu-id="f5638-114">Não pode ser nulo.</span><span class="sxs-lookup"><span data-stu-id="f5638-114">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f5638-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5638-115">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="f5638-116">Confira também</span><span class="sxs-lookup"><span data-stu-id="f5638-116">See also</span></span>

- [<span data-ttu-id="f5638-117">team</span><span class="sxs-lookup"><span data-stu-id="f5638-117">team</span></span>](team.md)

