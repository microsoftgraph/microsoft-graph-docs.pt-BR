---
title: tipo complexo internalSponsors
description: Identifica uma relação com outro usuário no locatário que será permitido como Aprovador.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c7ec468638de5e9a49cbf2f664eb7d05e3bef5b1
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331361"
---
# <a name="internalsponsors-complex-type"></a><span data-ttu-id="ddb8d-103">tipo complexo internalSponsors</span><span class="sxs-lookup"><span data-stu-id="ddb8d-103">internalSponsors complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddb8d-104">Usada no estágio de aprovação de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ddb8d-104">Used in the approval stage of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="ddb8d-105">É um subtipo de [userset](userset.md), no qual o valor `@odata.type` `#microsoft.graph.internalSponsors` indica que os patrocinadores internos da organização conectada do usuário solicitante sejam o aprovador.</span><span class="sxs-lookup"><span data-stu-id="ddb8d-105">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.internalSponsors` indicates that a requesting user's connected organization internal sponsors are to be the approver.</span></span> <span data-ttu-id="ddb8d-106">Esse aprovador só é aplicável a solicitações de usuários que fazem parte de uma organização conectada.</span><span class="sxs-lookup"><span data-stu-id="ddb8d-106">This approver is only applicable to requests from users who are part of a connected organization.</span></span>  <span data-ttu-id="ddb8d-107">Ao criar um estágio de aprovação de política de atribuição de pacote do Access com o internalSponsors, também inclua outro aprovador, como um único usuário ou membro de grupo, caso a organização conectada não tenha um patrocinador interno.</span><span class="sxs-lookup"><span data-stu-id="ddb8d-107">When creating an access package assignment policy approval stage with internalSponsors, also include another approver, such as a single user or group member, in case the connected organization does not have an internal sponsor.</span></span>

## <a name="properties"></a><span data-ttu-id="ddb8d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ddb8d-108">Properties</span></span>

| <span data-ttu-id="ddb8d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ddb8d-109">Property</span></span>                     | <span data-ttu-id="ddb8d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddb8d-110">Type</span></span>                      | <span data-ttu-id="ddb8d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddb8d-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="ddb8d-112">IsBackup</span><span class="sxs-lookup"><span data-stu-id="ddb8d-112">isBackup</span></span> | <span data-ttu-id="ddb8d-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="ddb8d-113">Boolean</span></span> | <span data-ttu-id="ddb8d-114">Indica se o patrocinador é um Aprovador de fallback de backup.</span><span class="sxs-lookup"><span data-stu-id="ddb8d-114">Indicates whether the sponsor is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ddb8d-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ddb8d-115">JSON representation</span></span>

<span data-ttu-id="ddb8d-116">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="ddb8d-116">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.internalSponsors",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "@odata.type": "#microsoft.graph.internalSponsors",
  "isBackup": false
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "internalSponsor complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
