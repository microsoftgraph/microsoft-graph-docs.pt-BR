---
title: Tipo complexo internalSponsors
description: Identifica uma relação com outro usuário no locatário que será permitido como aprovador.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 84c53bbeacde51afc88f5c0b4b5c13bc4f68b430
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760894"
---
# <a name="internalsponsors-complex-type"></a><span data-ttu-id="007a8-103">Tipo complexo internalSponsors</span><span class="sxs-lookup"><span data-stu-id="007a8-103">internalSponsors complex type</span></span>

<span data-ttu-id="007a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="007a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="007a8-105">Usado no estágio de aprovação de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="007a8-105">Used in the approval stage of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="007a8-106">É um subtipo de [userSet](userset.md), no qual o valor indica que os patrocinadores internos da organização conectada de um usuário solicitante devem `@odata.type` ser o `#microsoft.graph.internalSponsors` aprovador.</span><span class="sxs-lookup"><span data-stu-id="007a8-106">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.internalSponsors` indicates that a requesting user's connected organization internal sponsors are to be the approver.</span></span> <span data-ttu-id="007a8-107">Esse aprovador só se aplica a solicitações de usuários que fazem parte de uma organização conectada.</span><span class="sxs-lookup"><span data-stu-id="007a8-107">This approver is only applicable to requests from users who are part of a connected organization.</span></span>  <span data-ttu-id="007a8-108">Ao criar um estágio de aprovação da política de atribuição de pacote de acesso com internalSponsors, inclua também outro aprovador, como um único usuário ou membro do grupo, caso a organização conectada não tenha um patrocinador interno.</span><span class="sxs-lookup"><span data-stu-id="007a8-108">When creating an access package assignment policy approval stage with internalSponsors, also include another approver, such as a single user or group member, in case the connected organization does not have an internal sponsor.</span></span>

## <a name="properties"></a><span data-ttu-id="007a8-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="007a8-109">Properties</span></span>

| <span data-ttu-id="007a8-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="007a8-110">Property</span></span>                     | <span data-ttu-id="007a8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="007a8-111">Type</span></span>                      | <span data-ttu-id="007a8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="007a8-112">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="007a8-113">isBackup</span><span class="sxs-lookup"><span data-stu-id="007a8-113">isBackup</span></span> | <span data-ttu-id="007a8-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="007a8-114">Boolean</span></span> | <span data-ttu-id="007a8-115">Indica se o patrocinador é um aprovador de fallback de backup.</span><span class="sxs-lookup"><span data-stu-id="007a8-115">Indicates whether the sponsor is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="007a8-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="007a8-116">JSON representation</span></span>

<span data-ttu-id="007a8-117">A seguir está uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="007a8-117">The following is a JSON representation of the type.</span></span>

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


