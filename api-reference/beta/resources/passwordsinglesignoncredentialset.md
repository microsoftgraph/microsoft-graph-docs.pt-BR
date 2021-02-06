---
title: Tipo de recurso passwordSingleSignOnCredentialSet
description: Indica um conjunto de credenciais que definem completamente um fluxo de login de um usuário ou grupo para um aplicativo.
localization_priority: Normal
author: bharathramh92
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 95526942bcedfc20d983a8873699af6902482b2c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130871"
---
# <a name="passwordsinglesignoncredentialset-resource-type"></a><span data-ttu-id="34b90-103">Tipo de recurso passwordSingleSignOnCredentialSet</span><span class="sxs-lookup"><span data-stu-id="34b90-103">passwordSingleSignOnCredentialSet resource type</span></span>

<span data-ttu-id="34b90-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34b90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34b90-105">Indica um conjunto de credenciais que definem completamente um fluxo de login de um usuário ou grupo para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="34b90-105">Indicates a set of credentials that completely define a sign in flow for a user or group to an application.</span></span>

## <a name="properties"></a><span data-ttu-id="34b90-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34b90-106">Properties</span></span>

| <span data-ttu-id="34b90-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34b90-107">Property</span></span>     | <span data-ttu-id="34b90-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="34b90-108">Type</span></span>        | <span data-ttu-id="34b90-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="34b90-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="34b90-110">credenciais</span><span class="sxs-lookup"><span data-stu-id="34b90-110">credentials</span></span>|<span data-ttu-id="34b90-111">[coleção de](credential.md) credenciais</span><span class="sxs-lookup"><span data-stu-id="34b90-111">[credential](credential.md) collection</span></span>|<span data-ttu-id="34b90-112">Uma lista de objetos de credencial que definem o fluxo de login completo.</span><span class="sxs-lookup"><span data-stu-id="34b90-112">A list of credential objects that define the complete sign in flow.</span></span>|
|<span data-ttu-id="34b90-113">id</span><span class="sxs-lookup"><span data-stu-id="34b90-113">id</span></span>|<span data-ttu-id="34b90-114">String</span><span class="sxs-lookup"><span data-stu-id="34b90-114">String</span></span>|<span data-ttu-id="34b90-115">A ID do usuário ou grupo ao que esse conjunto de credenciais pertence.</span><span class="sxs-lookup"><span data-stu-id="34b90-115">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="34b90-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34b90-116">JSON representation</span></span>

<span data-ttu-id="34b90-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34b90-117">The following is a JSON representation of the resource.</span></span>

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


