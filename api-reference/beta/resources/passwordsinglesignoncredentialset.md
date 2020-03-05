---
title: tipo de recurso passwordSingleSignOnCredentialSet
description: Indica um conjunto de credenciais que definem completamente um fluxo de entrada para um usuário ou grupo para um aplicativo.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9191362f0e6c98d57c609445fbe1caf3bdd775a2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522001"
---
# <a name="passwordsinglesignoncredentialset-resource-type"></a><span data-ttu-id="b25a8-103">tipo de recurso passwordSingleSignOnCredentialSet</span><span class="sxs-lookup"><span data-stu-id="b25a8-103">passwordSingleSignOnCredentialSet resource type</span></span>

<span data-ttu-id="b25a8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b25a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b25a8-105">Indica um conjunto de credenciais que definem completamente um fluxo de entrada para um usuário ou grupo para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b25a8-105">Indicates a set of credentials that completely define a sign in flow for a user or group to an application.</span></span>

## <a name="properties"></a><span data-ttu-id="b25a8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b25a8-106">Properties</span></span>

| <span data-ttu-id="b25a8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b25a8-107">Property</span></span>     | <span data-ttu-id="b25a8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b25a8-108">Type</span></span>        | <span data-ttu-id="b25a8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b25a8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b25a8-110">las</span><span class="sxs-lookup"><span data-stu-id="b25a8-110">credentials</span></span>|<span data-ttu-id="b25a8-111">coleção [Credential](credential.md)</span><span class="sxs-lookup"><span data-stu-id="b25a8-111">[credential](credential.md) collection</span></span>|<span data-ttu-id="b25a8-112">Uma lista de objetos de credencial que definem o fluxo de entrada completo.</span><span class="sxs-lookup"><span data-stu-id="b25a8-112">A list of credential objects that define the complete sign in flow.</span></span>|
|<span data-ttu-id="b25a8-113">id</span><span class="sxs-lookup"><span data-stu-id="b25a8-113">id</span></span>|<span data-ttu-id="b25a8-114">String</span><span class="sxs-lookup"><span data-stu-id="b25a8-114">String</span></span>|<span data-ttu-id="b25a8-115">A ID do usuário ou grupo ao qual esse conjunto de credenciais pertence.</span><span class="sxs-lookup"><span data-stu-id="b25a8-115">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b25a8-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b25a8-116">JSON representation</span></span>

<span data-ttu-id="b25a8-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b25a8-117">The following is a JSON representation of the resource.</span></span>

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
