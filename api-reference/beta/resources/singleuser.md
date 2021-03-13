---
title: tipo complexo singleUser
description: Identifica um usuário no locatário que será permitido como solicitante, aprovador ou revisor.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8e1982eef048e1f68f579df7f2ebc6b0975f2f0b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761041"
---
# <a name="singleuser-complex-type"></a><span data-ttu-id="0608d-103">tipo complexo singleUser</span><span class="sxs-lookup"><span data-stu-id="0608d-103">singleUser complex type</span></span>

<span data-ttu-id="0608d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0608d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0608d-105">Usado nas configurações de solicitação, aprovação e revisão de atribuição de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0608d-105">Used in the request, approval, and assignment review settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="0608d-106">O valor indica que esse conjunto de usuários identifica um usuário específico no locatário que será permitido como  `@odata.type` `#microsoft.graph.singleUser` solicitante, aprovador ou revisor.</span><span class="sxs-lookup"><span data-stu-id="0608d-106">The  `@odata.type` value `#microsoft.graph.singleUser` indicates that this user set identifies a specific user in the tenant who will be allowed as a requestor, approver, or reviewer.</span></span>

## <a name="properties"></a><span data-ttu-id="0608d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0608d-107">Properties</span></span>

<span data-ttu-id="0608d-108">Esse tipo tem as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="0608d-108">This type has the following properties:</span></span>

| <span data-ttu-id="0608d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0608d-109">Property</span></span>                     | <span data-ttu-id="0608d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0608d-110">Type</span></span>                      | <span data-ttu-id="0608d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0608d-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="0608d-112">id</span><span class="sxs-lookup"><span data-stu-id="0608d-112">id</span></span> |<span data-ttu-id="0608d-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0608d-113">String</span></span> | <span data-ttu-id="0608d-114">A ID do usuário no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0608d-114">The ID of the user in Azure AD.</span></span> |
| <span data-ttu-id="0608d-115">descrição</span><span class="sxs-lookup"><span data-stu-id="0608d-115">description</span></span> |<span data-ttu-id="0608d-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0608d-116">String</span></span> | <span data-ttu-id="0608d-117">O nome do usuário no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0608d-117">The name of the user in Azure AD.</span></span> <span data-ttu-id="0608d-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0608d-118">Read only.</span></span> |
| <span data-ttu-id="0608d-119">isBackup</span><span class="sxs-lookup"><span data-stu-id="0608d-119">isBackup</span></span> | <span data-ttu-id="0608d-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="0608d-120">Boolean</span></span> | <span data-ttu-id="0608d-121">Para um **singleUser** em um estágio de aprovação, indica se o usuário é um aprovador de fallback de backup.</span><span class="sxs-lookup"><span data-stu-id="0608d-121">For a **singleUser** in an approval stage, indicates whether the user is a backup fallback approver.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0608d-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0608d-122">JSON representation</span></span>

<span data-ttu-id="0608d-123">A seguir está uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="0608d-123">The following is a JSON representation of the type.</span></span>

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


