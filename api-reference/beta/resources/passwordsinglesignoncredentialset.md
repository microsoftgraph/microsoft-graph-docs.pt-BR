---
title: tipo de recurso passwordSingleSignOnCredentialSet
description: Indica um conjunto de credenciais que definem completamente um fluxo de entrada para um usuário ou grupo para um aplicativo.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 87aafa6e21171088f9b4b5eac318f6c9551e18ee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998198"
---
# <a name="passwordsinglesignoncredentialset-resource-type"></a><span data-ttu-id="93e69-103">tipo de recurso passwordSingleSignOnCredentialSet</span><span class="sxs-lookup"><span data-stu-id="93e69-103">passwordSingleSignOnCredentialSet resource type</span></span>

<span data-ttu-id="93e69-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93e69-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93e69-105">Indica um conjunto de credenciais que definem completamente um fluxo de entrada para um usuário ou grupo para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="93e69-105">Indicates a set of credentials that completely define a sign in flow for a user or group to an application.</span></span>

## <a name="properties"></a><span data-ttu-id="93e69-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93e69-106">Properties</span></span>

| <span data-ttu-id="93e69-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93e69-107">Property</span></span>     | <span data-ttu-id="93e69-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="93e69-108">Type</span></span>        | <span data-ttu-id="93e69-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="93e69-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="93e69-110">las</span><span class="sxs-lookup"><span data-stu-id="93e69-110">credentials</span></span>|<span data-ttu-id="93e69-111">coleção [Credential](credential.md)</span><span class="sxs-lookup"><span data-stu-id="93e69-111">[credential](credential.md) collection</span></span>|<span data-ttu-id="93e69-112">Uma lista de objetos de credencial que definem o fluxo de entrada completo.</span><span class="sxs-lookup"><span data-stu-id="93e69-112">A list of credential objects that define the complete sign in flow.</span></span>|
|<span data-ttu-id="93e69-113">id</span><span class="sxs-lookup"><span data-stu-id="93e69-113">id</span></span>|<span data-ttu-id="93e69-114">String</span><span class="sxs-lookup"><span data-stu-id="93e69-114">String</span></span>|<span data-ttu-id="93e69-115">A ID do usuário ou grupo ao qual esse conjunto de credenciais pertence.</span><span class="sxs-lookup"><span data-stu-id="93e69-115">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="93e69-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93e69-116">JSON representation</span></span>

<span data-ttu-id="93e69-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93e69-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordSingleSignOnCredentialSet",
  "baseType": null
}-->

```json
{
  "credentials": [{"@odata.type": "microsoft.graph.credential"}],
  "id": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordSingleSignOnCredentialSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


