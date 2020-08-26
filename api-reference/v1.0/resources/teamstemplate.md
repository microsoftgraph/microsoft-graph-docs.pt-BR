---
title: tipo de recurso Teams
description: Descreve a entidade Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c32c8cfa770bd7633915e0e8f9b6d371458d4173
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873402"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="c85ab-103">tipo de recurso Teams</span><span class="sxs-lookup"><span data-stu-id="c85ab-103">teamsTemplate resource type</span></span>

<span data-ttu-id="c85ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c85ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c85ab-105">Um modelo de equipe é um gráfico para a criação de uma [equipe](../resources/team.md) no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c85ab-105">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="c85ab-106">Um modelo especifica a estrutura, as configurações e até o conteúdo que deve ser provisionado em uma nova equipe criada usando o modelo.</span><span class="sxs-lookup"><span data-stu-id="c85ab-106">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="c85ab-107">A Microsoft fornece um pacote de modelos básicos e os clientes podem salvar seus próprios modelos personalizados.</span><span class="sxs-lookup"><span data-stu-id="c85ab-107">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="c85ab-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c85ab-108">Properties</span></span>

| <span data-ttu-id="c85ab-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c85ab-109">Property</span></span>            | <span data-ttu-id="c85ab-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c85ab-110">Type</span></span>     | <span data-ttu-id="c85ab-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c85ab-111">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="c85ab-112">id</span><span class="sxs-lookup"><span data-stu-id="c85ab-112">id</span></span>                  | <span data-ttu-id="c85ab-113">String</span><span class="sxs-lookup"><span data-stu-id="c85ab-113">String</span></span>   | <span data-ttu-id="c85ab-114">Identificador exclusivo do modelo.</span><span class="sxs-lookup"><span data-stu-id="c85ab-114">Unique identifier of the template.</span></span> <span data-ttu-id="c85ab-115">Não pode ser nulo.</span><span class="sxs-lookup"><span data-stu-id="c85ab-115">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c85ab-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c85ab-116">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="c85ab-117">Confira também</span><span class="sxs-lookup"><span data-stu-id="c85ab-117">See also</span></span>

- [<span data-ttu-id="c85ab-118">team</span><span class="sxs-lookup"><span data-stu-id="c85ab-118">team</span></span>](team.md)

