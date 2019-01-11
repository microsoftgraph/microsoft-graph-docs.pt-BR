---
title: tipo de recurso de teamsTemplate
description: Descreve a entidade teamsTemplate.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 6e847c7ef0b13dd9c4281c17939164128be8b6a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818869"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="a2c65-103">tipo de recurso de teamsTemplate</span><span class="sxs-lookup"><span data-stu-id="a2c65-103">teamsTemplate resource type</span></span>

> <span data-ttu-id="a2c65-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a2c65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2c65-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a2c65-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a2c65-106">Um modelo de equipe é um blueprint para a criação de uma [equipe](../resources/team.md) no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a2c65-106">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="a2c65-107">Um modelo especifica a estrutura, configurações e até mesmo conteúdo que deve ser provisionado em uma nova criada usando o modelo de equipe.</span><span class="sxs-lookup"><span data-stu-id="a2c65-107">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="a2c65-108">A Microsoft fornece um pacote de modelos de base e os clientes podem salvar seus próprios modelos personalizados.</span><span class="sxs-lookup"><span data-stu-id="a2c65-108">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="a2c65-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2c65-109">Properties</span></span>

| <span data-ttu-id="a2c65-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2c65-110">Property</span></span>            | <span data-ttu-id="a2c65-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2c65-111">Type</span></span>     | <span data-ttu-id="a2c65-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2c65-112">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="a2c65-113">id</span><span class="sxs-lookup"><span data-stu-id="a2c65-113">id</span></span>                  | <span data-ttu-id="a2c65-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2c65-114">String</span></span>   | <span data-ttu-id="a2c65-115">Identificador exclusivo do modelo.</span><span class="sxs-lookup"><span data-stu-id="a2c65-115">Unique identifier of the template.</span></span> <span data-ttu-id="a2c65-116">Não pode ser nula.</span><span class="sxs-lookup"><span data-stu-id="a2c65-116">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a2c65-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2c65-117">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="a2c65-118">Confira também</span><span class="sxs-lookup"><span data-stu-id="a2c65-118">See also</span></span>

- [<span data-ttu-id="a2c65-119">equipe</span><span class="sxs-lookup"><span data-stu-id="a2c65-119">team</span></span>](team.md)

