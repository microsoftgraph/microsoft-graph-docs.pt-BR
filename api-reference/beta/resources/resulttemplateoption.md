---
title: Tipo de recurso resultTemplateOption
description: Fornece as opções de layouts de exibição de pesquisa para resultados de pesquisa de conectores de renderização.
localization_priority: Normal
author: cristianv-ms
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 404051f4eeee68ca3d5f5eb3ac6b84a23a331515
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211201"
---
# <a name="resulttemplateoption-resource-type"></a><span data-ttu-id="e68c6-103">Tipo de recurso resultTemplateOption</span><span class="sxs-lookup"><span data-stu-id="e68c6-103">resultTemplateOption resource type</span></span>

<span data-ttu-id="e68c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e68c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e68c6-105">Fornece as opções de modelos de resultados de pesquisa para resultados de pesquisa de conectores de renderização.</span><span class="sxs-lookup"><span data-stu-id="e68c6-105">Provides the search result templates options for render connectors search results.</span></span>

## <a name="properties"></a><span data-ttu-id="e68c6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e68c6-106">Properties</span></span>

| <span data-ttu-id="e68c6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e68c6-107">Property</span></span>     | <span data-ttu-id="e68c6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e68c6-108">Type</span></span>        | <span data-ttu-id="e68c6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e68c6-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e68c6-110">enableResultTemplate</span><span class="sxs-lookup"><span data-stu-id="e68c6-110">enableResultTemplate</span></span>|<span data-ttu-id="e68c6-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="e68c6-111">Boolean</span></span>|<span data-ttu-id="e68c6-112">Indica se os layouts de exibição de pesquisa estão habilitados.</span><span class="sxs-lookup"><span data-stu-id="e68c6-112">Indicates whether search display layouts are enabled.</span></span> <span data-ttu-id="e68c6-113">Se habilitado, o usuário receberá o modelo de resultado para renderizar o conteúdo dos resultados da pesquisa na **propriedade resultTemplates** da [resposta](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="e68c6-113">If enabled, the user will get the result template to render the search results content in the **resultTemplates** property of the [response](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="e68c6-114">O modelo de resultado baseia-se em [Cartões Adaptáveis.](https://adaptivecards.io/)</span><span class="sxs-lookup"><span data-stu-id="e68c6-114">The result template is based on [Adaptive Cards](https://adaptivecards.io/).</span></span> <span data-ttu-id="e68c6-115">Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="e68c6-115">This property is optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e68c6-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e68c6-116">JSON representation</span></span>

<span data-ttu-id="e68c6-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e68c6-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultTemplateOption",
  "baseType": null
}-->

```json
 {
    "enableResultTemplate": true
 }
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resultTemplateOption resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
