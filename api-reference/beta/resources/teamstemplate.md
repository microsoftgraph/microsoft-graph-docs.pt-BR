---
title: tipo de recurso Teams
description: Descreve a entidade Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5fc40b9c2a5789c5bcd7ab5794e41c715223eff3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046382"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="bfe41-103">tipo de recurso Teams</span><span class="sxs-lookup"><span data-stu-id="bfe41-103">teamsTemplate resource type</span></span>

<span data-ttu-id="bfe41-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfe41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfe41-105">Um modelo de equipe é um gráfico para a criação de uma [equipe](../resources/team.md) no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="bfe41-105">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="bfe41-106">Um modelo especifica a estrutura, as configurações e até o conteúdo que deve ser provisionado em uma nova equipe criada usando o modelo.</span><span class="sxs-lookup"><span data-stu-id="bfe41-106">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="bfe41-107">A Microsoft fornece um pacote de modelos básicos e os clientes podem salvar seus próprios modelos personalizados.</span><span class="sxs-lookup"><span data-stu-id="bfe41-107">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="bfe41-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bfe41-108">Properties</span></span>

| <span data-ttu-id="bfe41-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bfe41-109">Property</span></span>            | <span data-ttu-id="bfe41-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfe41-110">Type</span></span>     | <span data-ttu-id="bfe41-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfe41-111">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="bfe41-112">id</span><span class="sxs-lookup"><span data-stu-id="bfe41-112">id</span></span>                  | <span data-ttu-id="bfe41-113">String</span><span class="sxs-lookup"><span data-stu-id="bfe41-113">String</span></span>   | <span data-ttu-id="bfe41-114">Identificador exclusivo do modelo.</span><span class="sxs-lookup"><span data-stu-id="bfe41-114">Unique identifier of the template.</span></span> <span data-ttu-id="bfe41-115">Não pode ser nulo.</span><span class="sxs-lookup"><span data-stu-id="bfe41-115">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bfe41-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bfe41-116">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="bfe41-117">Confira também</span><span class="sxs-lookup"><span data-stu-id="bfe41-117">See also</span></span>

- [<span data-ttu-id="bfe41-118">team</span><span class="sxs-lookup"><span data-stu-id="bfe41-118">team</span></span>](team.md)



