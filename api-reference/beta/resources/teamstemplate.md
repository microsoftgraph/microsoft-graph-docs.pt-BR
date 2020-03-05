---
title: tipo de recurso Teams
description: Descreve a entidade Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 77101c756e09b4ce2356da2384f2c50b119ae856
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519831"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="7e5c4-103">tipo de recurso Teams</span><span class="sxs-lookup"><span data-stu-id="7e5c4-103">teamsTemplate resource type</span></span>

<span data-ttu-id="7e5c4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7e5c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e5c4-105">Um modelo de equipe é um gráfico para a criação de uma [equipe](../resources/team.md) no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7e5c4-105">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="7e5c4-106">Um modelo especifica a estrutura, as configurações e até o conteúdo que deve ser provisionado em uma nova equipe criada usando o modelo.</span><span class="sxs-lookup"><span data-stu-id="7e5c4-106">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="7e5c4-107">A Microsoft fornece um pacote de modelos básicos e os clientes podem salvar seus próprios modelos personalizados.</span><span class="sxs-lookup"><span data-stu-id="7e5c4-107">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="7e5c4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7e5c4-108">Properties</span></span>

| <span data-ttu-id="7e5c4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e5c4-109">Property</span></span>            | <span data-ttu-id="7e5c4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e5c4-110">Type</span></span>     | <span data-ttu-id="7e5c4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e5c4-111">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="7e5c4-112">id</span><span class="sxs-lookup"><span data-stu-id="7e5c4-112">id</span></span>                  | <span data-ttu-id="7e5c4-113">String</span><span class="sxs-lookup"><span data-stu-id="7e5c4-113">String</span></span>   | <span data-ttu-id="7e5c4-114">Identificador exclusivo do modelo.</span><span class="sxs-lookup"><span data-stu-id="7e5c4-114">Unique identifier of the template.</span></span> <span data-ttu-id="7e5c4-115">Não pode ser nulo.</span><span class="sxs-lookup"><span data-stu-id="7e5c4-115">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7e5c4-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7e5c4-116">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="7e5c4-117">Confira também</span><span class="sxs-lookup"><span data-stu-id="7e5c4-117">See also</span></span>

- [<span data-ttu-id="7e5c4-118">team</span><span class="sxs-lookup"><span data-stu-id="7e5c4-118">team</span></span>](team.md)

