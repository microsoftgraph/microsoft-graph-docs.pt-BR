---
title: tipo complexo externalSponsors
description: Identifica uma relação com outro usuário no locatário que será permitido como aprovador.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 361ac6ff85d5b4462b39aa10e4f978ce7d486e40
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761867"
---
# <a name="externalsponsors-complex-type"></a><span data-ttu-id="f0b00-103">tipo complexo externalSponsors</span><span class="sxs-lookup"><span data-stu-id="f0b00-103">externalSponsors complex type</span></span>

<span data-ttu-id="f0b00-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0b00-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0b00-105">Usado no estágio de aprovação de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f0b00-105">Used in the approval stage of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="f0b00-106">É um subtipo de [userSet](userset.md), no qual o valor indica que os patrocinadores externos de uma organização conectada do usuário solicitante devem `@odata.type` ser o `#microsoft.graph.externalSponsors` aprovador.</span><span class="sxs-lookup"><span data-stu-id="f0b00-106">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.externalSponsors` indicates that a requesting user's connected organization external sponsors are to be the approver.</span></span> <span data-ttu-id="f0b00-107">Esse aprovador só se aplica a solicitações de usuários que fazem parte de uma organização conectada.</span><span class="sxs-lookup"><span data-stu-id="f0b00-107">This approver is only applicable to requests from users who are part of a connected organization.</span></span>  <span data-ttu-id="f0b00-108">Ao criar um estágio de aprovação da política de atribuição de pacote de acesso com externalSponsors, inclua também outro aprovador, como um único usuário ou membro do grupo, caso a organização conectada não tenha um patrocinador externo.</span><span class="sxs-lookup"><span data-stu-id="f0b00-108">When creating an access package assignment policy approval stage with externalSponsors, also include another approver, such as a single user or group member, in case the connected organization does not have an external sponsor.</span></span>

## <a name="properties"></a><span data-ttu-id="f0b00-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0b00-109">Properties</span></span>

| <span data-ttu-id="f0b00-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0b00-110">Property</span></span>                     | <span data-ttu-id="f0b00-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0b00-111">Type</span></span>                      | <span data-ttu-id="f0b00-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0b00-112">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="f0b00-113">isBackup</span><span class="sxs-lookup"><span data-stu-id="f0b00-113">isBackup</span></span> | <span data-ttu-id="f0b00-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0b00-114">Boolean</span></span> | <span data-ttu-id="f0b00-115">Indica se o patrocinador é um aprovador de fallback de backup.</span><span class="sxs-lookup"><span data-stu-id="f0b00-115">Indicates whether the sponsor is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f0b00-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0b00-116">JSON representation</span></span>

<span data-ttu-id="f0b00-117">A seguir está uma representação JSON desse tipo.</span><span class="sxs-lookup"><span data-stu-id="f0b00-117">The following is a JSON representation of this type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalSponsors",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "@odata.type": "#microsoft.graph.externalSponsors",
  "isBackup": false
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalSponsor complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


