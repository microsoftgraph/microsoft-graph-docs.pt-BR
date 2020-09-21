---
title: tipo complexo Únicousuário
description: Identifica um usuário no locatário que será permitido como solicitante, Aprovador ou revisor.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fb6b665814281629836f4c5148b567de776ef2ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067122"
---
# <a name="singleuser-complex-type"></a><span data-ttu-id="c8d16-103">tipo complexo Únicousuário</span><span class="sxs-lookup"><span data-stu-id="c8d16-103">singleUser complex type</span></span>

<span data-ttu-id="c8d16-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8d16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8d16-105">Usado nas configurações de solicitação, aprovação e revisão de atribuição de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c8d16-105">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="c8d16-106">O  `@odata.type` valor `#microsoft.graph.singleUser` indica que este conjunto de usuários identifica um usuário específico no locatário que será permitido como solicitante, Aprovador ou revisor.</span><span class="sxs-lookup"><span data-stu-id="c8d16-106">The  `@odata.type` value `#microsoft.graph.singleUser` indicates that this user set identifies a specific user in the tenant who will be allowed as a requestor, approver, or reviewer.</span></span>

## <a name="properties"></a><span data-ttu-id="c8d16-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8d16-107">Properties</span></span>

<span data-ttu-id="c8d16-108">Este tipo tem as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="c8d16-108">This type has the following properties:</span></span>

| <span data-ttu-id="c8d16-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8d16-109">Property</span></span>                     | <span data-ttu-id="c8d16-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8d16-110">Type</span></span>                      | <span data-ttu-id="c8d16-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8d16-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="c8d16-112">id</span><span class="sxs-lookup"><span data-stu-id="c8d16-112">id</span></span> |<span data-ttu-id="c8d16-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8d16-113">String</span></span> | <span data-ttu-id="c8d16-114">A ID do usuário no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c8d16-114">The ID of the user in Azure AD.</span></span> |
| <span data-ttu-id="c8d16-115">description</span><span class="sxs-lookup"><span data-stu-id="c8d16-115">description</span></span> |<span data-ttu-id="c8d16-116">String</span><span class="sxs-lookup"><span data-stu-id="c8d16-116">String</span></span> | <span data-ttu-id="c8d16-117">O nome do usuário no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c8d16-117">The name of the user in Azure AD.</span></span> <span data-ttu-id="c8d16-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c8d16-118">Read only.</span></span> |
| <span data-ttu-id="c8d16-119">IsBackup</span><span class="sxs-lookup"><span data-stu-id="c8d16-119">isBackup</span></span> | <span data-ttu-id="c8d16-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="c8d16-120">Boolean</span></span> | <span data-ttu-id="c8d16-121">Para um **únicousuário** em um estágio de aprovação, indica se o usuário é um Aprovador de fallback de backup.</span><span class="sxs-lookup"><span data-stu-id="c8d16-121">For a **singleUser** in an approval stage, indicates whether the user is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c8d16-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8d16-122">JSON representation</span></span>

<span data-ttu-id="c8d16-123">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="c8d16-123">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.singleUser",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "isBackup": false,
  "id": "string (identifier)",
  "description": "string"
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "singleUser complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


