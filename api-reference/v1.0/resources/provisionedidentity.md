---
title: Tipo de recurso provisionedIdentity
description: Descreve a identidade associada ao evento de resumo do objeto de provisionamento.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 083609787920d840d8576d1c2a7cd5e39945768c
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241503"
---
# <a name="provisionedidentity-resource-type"></a><span data-ttu-id="1c727-103">Tipo de recurso provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="1c727-103">provisionedIdentity resource type</span></span>

<span data-ttu-id="1c727-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c727-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="1c727-105">Descreve a identidade associada ao evento de resumo do objeto de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="1c727-105">Describes the identity associated with the provisioning object summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="1c727-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1c727-106">Properties</span></span>

| <span data-ttu-id="1c727-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c727-107">Property</span></span>     | <span data-ttu-id="1c727-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c727-108">Type</span></span>        | <span data-ttu-id="1c727-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c727-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1c727-110">detalhes</span><span class="sxs-lookup"><span data-stu-id="1c727-110">details</span></span>|[<span data-ttu-id="1c727-111">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="1c727-111">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="1c727-112">Detalhes da identidade.</span><span class="sxs-lookup"><span data-stu-id="1c727-112">Details of the identity.</span></span>|
|<span data-ttu-id="1c727-113">displayName</span><span class="sxs-lookup"><span data-stu-id="1c727-113">displayName</span></span>|<span data-ttu-id="1c727-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c727-114">String</span></span>|<span data-ttu-id="1c727-115">Nome de exibição da identidade.</span><span class="sxs-lookup"><span data-stu-id="1c727-115">Display name of the identity.</span></span> |
|<span data-ttu-id="1c727-116">id</span><span class="sxs-lookup"><span data-stu-id="1c727-116">id</span></span>|<span data-ttu-id="1c727-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c727-117">String</span></span>|<span data-ttu-id="1c727-118">Identifica exclusivamente a identidade.</span><span class="sxs-lookup"><span data-stu-id="1c727-118">Uniquely identifies the identity.</span></span>|
|<span data-ttu-id="1c727-119">identityType</span><span class="sxs-lookup"><span data-stu-id="1c727-119">identityType</span></span>|<span data-ttu-id="1c727-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c727-120">String</span></span>|<span data-ttu-id="1c727-121">Tipo de identidade que foi provisionado, como "usuário" ou "grupo".</span><span class="sxs-lookup"><span data-stu-id="1c727-121">Type of identity that has been provisioned, such as 'user' or 'group'.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1c727-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1c727-122">JSON representation</span></span>

<span data-ttu-id="1c727-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1c727-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedIdentity",
  "baseType": null
}-->

```json
{
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "displayName": "String",
  "id": "String",
  "identityType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


