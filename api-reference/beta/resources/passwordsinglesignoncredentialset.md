---
title: tipo de recurso passwordSingleSignOnCredentialSet
description: Indica um conjunto de credenciais que definem completamente um fluxo de entrada para um usuário ou grupo para um aplicativo.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6293c6a2fbdffd124a8e011bd00a22c30efa77e5
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658790"
---
# <a name="passwordsinglesignoncredentialset-resource-type"></a><span data-ttu-id="462a2-103">tipo de recurso passwordSingleSignOnCredentialSet</span><span class="sxs-lookup"><span data-stu-id="462a2-103">passwordSingleSignOnCredentialSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="462a2-104">Indica um conjunto de credenciais que definem completamente um fluxo de entrada para um usuário ou grupo para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="462a2-104">Indicates a set of credentials that completely define a sign in flow for a user or group to an application.</span></span>

## <a name="properties"></a><span data-ttu-id="462a2-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="462a2-105">Properties</span></span>

| <span data-ttu-id="462a2-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="462a2-106">Property</span></span>     | <span data-ttu-id="462a2-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="462a2-107">Type</span></span>        | <span data-ttu-id="462a2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="462a2-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="462a2-109">las</span><span class="sxs-lookup"><span data-stu-id="462a2-109">credentials</span></span>|<span data-ttu-id="462a2-110">coleção [Credential](credential.md)</span><span class="sxs-lookup"><span data-stu-id="462a2-110">[credential](credential.md) collection</span></span>|<span data-ttu-id="462a2-111">Uma lista de objetos de credencial que definem o fluxo de entrada completo.</span><span class="sxs-lookup"><span data-stu-id="462a2-111">A list of credential objects that define the complete sign in flow.</span></span>|
|<span data-ttu-id="462a2-112">id</span><span class="sxs-lookup"><span data-stu-id="462a2-112">id</span></span>|<span data-ttu-id="462a2-113">String</span><span class="sxs-lookup"><span data-stu-id="462a2-113">String</span></span>|<span data-ttu-id="462a2-114">A ID do usuário ou grupo ao qual esse conjunto de credenciais pertence.</span><span class="sxs-lookup"><span data-stu-id="462a2-114">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="462a2-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="462a2-115">JSON representation</span></span>

<span data-ttu-id="462a2-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="462a2-116">The following is a JSON representation of the resource.</span></span>

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
