---
title: tipo complexo Únicousuário
description: Identifica um usuário no locatário que será permitido como solicitante, Aprovador ou revisor.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0d4db47278051dd79b697dc352549b95b872e4aa
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331338"
---
# <a name="singleuser-complex-type"></a><span data-ttu-id="557a1-103">tipo complexo Únicousuário</span><span class="sxs-lookup"><span data-stu-id="557a1-103">singleUser complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="557a1-104">Usado nas configurações de solicitação, aprovação e revisão de atribuição de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="557a1-104">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="557a1-105">O `@odata.type` valor `#microsoft.graph.singleUser` indica que este conjunto de usuários identifica um usuário específico no locatário que será permitido como solicitante, Aprovador ou revisor.</span><span class="sxs-lookup"><span data-stu-id="557a1-105">The  `@odata.type` value `#microsoft.graph.singleUser` indicates that this user set identifies a specific user in the tenant who will be allowed as a requestor, approver, or reviewer.</span></span>

## <a name="properties"></a><span data-ttu-id="557a1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="557a1-106">Properties</span></span>

<span data-ttu-id="557a1-107">Este tipo tem as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="557a1-107">This type has the following properties:</span></span>

| <span data-ttu-id="557a1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="557a1-108">Property</span></span>                     | <span data-ttu-id="557a1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="557a1-109">Type</span></span>                      | <span data-ttu-id="557a1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="557a1-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="557a1-111">id</span><span class="sxs-lookup"><span data-stu-id="557a1-111">id</span></span> |<span data-ttu-id="557a1-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="557a1-112">String</span></span> | <span data-ttu-id="557a1-113">A ID do usuário no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="557a1-113">The ID of the user in Azure AD.</span></span> |
| <span data-ttu-id="557a1-114">descrição</span><span class="sxs-lookup"><span data-stu-id="557a1-114">description</span></span> |<span data-ttu-id="557a1-115">String</span><span class="sxs-lookup"><span data-stu-id="557a1-115">String</span></span> | <span data-ttu-id="557a1-116">O nome do usuário no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="557a1-116">The name of the user in Azure AD.</span></span> <span data-ttu-id="557a1-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="557a1-117">Read only.</span></span> |
| <span data-ttu-id="557a1-118">IsBackup</span><span class="sxs-lookup"><span data-stu-id="557a1-118">isBackup</span></span> | <span data-ttu-id="557a1-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="557a1-119">Boolean</span></span> | <span data-ttu-id="557a1-120">Para um **únicousuário** em um estágio de aprovação, indica se o usuário é um Aprovador de fallback de backup.</span><span class="sxs-lookup"><span data-stu-id="557a1-120">For a **singleUser** in an approval stage, indicates whether the user is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="557a1-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="557a1-121">JSON representation</span></span>

<span data-ttu-id="557a1-122">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="557a1-122">The following is a JSON representation of the type.</span></span>

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
