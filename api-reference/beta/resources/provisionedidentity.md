---
title: Tipo de recurso provisionedIdentity
description: Descreve a identidade associada ao evento de resumo do objeto de provisionamento.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 2de68bdce990a6a541a5c284672541669cfdebea
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761104"
---
# <a name="provisionedidentity-resource-type"></a><span data-ttu-id="7beb7-103">Tipo de recurso provisionedIdentity</span><span class="sxs-lookup"><span data-stu-id="7beb7-103">provisionedIdentity resource type</span></span>

<span data-ttu-id="7beb7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7beb7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7beb7-105">Descreve a identidade associada ao evento de resumo do objeto de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="7beb7-105">Describes the identity associated with the provisioning object summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="7beb7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7beb7-106">Properties</span></span>

| <span data-ttu-id="7beb7-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7beb7-107">Property</span></span>     | <span data-ttu-id="7beb7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7beb7-108">Type</span></span>        | <span data-ttu-id="7beb7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7beb7-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7beb7-110">detalhes</span><span class="sxs-lookup"><span data-stu-id="7beb7-110">details</span></span>|[<span data-ttu-id="7beb7-111">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="7beb7-111">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="7beb7-112">Detalhes da identidade.</span><span class="sxs-lookup"><span data-stu-id="7beb7-112">Details of the identity.</span></span>|
|<span data-ttu-id="7beb7-113">displayName</span><span class="sxs-lookup"><span data-stu-id="7beb7-113">displayName</span></span>|<span data-ttu-id="7beb7-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7beb7-114">String</span></span>|<span data-ttu-id="7beb7-115">Nome de exibição da identidade.</span><span class="sxs-lookup"><span data-stu-id="7beb7-115">Display name of the identity.</span></span> |
|<span data-ttu-id="7beb7-116">id</span><span class="sxs-lookup"><span data-stu-id="7beb7-116">id</span></span>|<span data-ttu-id="7beb7-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7beb7-117">String</span></span>|<span data-ttu-id="7beb7-118">Identifica exclusivamente a identidade.</span><span class="sxs-lookup"><span data-stu-id="7beb7-118">Uniquely identifies the identity.</span></span>|
|<span data-ttu-id="7beb7-119">identityType</span><span class="sxs-lookup"><span data-stu-id="7beb7-119">identityType</span></span>|<span data-ttu-id="7beb7-120">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="7beb7-120">String</span></span>|<span data-ttu-id="7beb7-121">Tipo de identidade que foi provisionado, como "usuário" ou "grupo".</span><span class="sxs-lookup"><span data-stu-id="7beb7-121">Type of identity that has been provisioned, such as 'user' or 'group'.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7beb7-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7beb7-122">JSON representation</span></span>

<span data-ttu-id="7beb7-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7beb7-123">The following is a JSON representation of the resource.</span></span>

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


