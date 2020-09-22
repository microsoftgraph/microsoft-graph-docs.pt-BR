---
title: tipo complexo connectedOrganizationMembers
description: O tipo connectedOrganizationMembers identifica uma coleção de usuários no locatário que serão permitidos como solicitante, Aprovador ou revisor.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d2df6b91ebcbc65f03ee39103768bdfad04df62f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027192"
---
# <a name="connectedorganizationmembers-complex-type"></a><span data-ttu-id="3ce4a-103">tipo complexo connectedOrganizationMembers</span><span class="sxs-lookup"><span data-stu-id="3ce4a-103">connectedOrganizationMembers complex type</span></span>

<span data-ttu-id="3ce4a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ce4a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ce4a-105">Usado nas configurações de solicitação de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3ce4a-105">Used in the request settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="3ce4a-106">O `@odata.type` valor `#microsoft.graph.connectedOrganizationMembers` indica que esse tipo identifica uma coleção de usuários, os que estão associados a uma [organização conectada](connectedorganization.md), que terá permissão para solicitar um pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="3ce4a-106">The `@odata.type` value `#microsoft.graph.connectedOrganizationMembers` indicates that this type identifies a collection of users, those who are associated with a [connected organization](connectedorganization.md), who will be allowed to request an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="3ce4a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ce4a-107">Properties</span></span>

<span data-ttu-id="3ce4a-108">Este tipo tem as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="3ce4a-108">This type has the following properties:</span></span>

| <span data-ttu-id="3ce4a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ce4a-109">Property</span></span>                     | <span data-ttu-id="3ce4a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ce4a-110">Type</span></span>                      | <span data-ttu-id="3ce4a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ce4a-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="3ce4a-112">id</span><span class="sxs-lookup"><span data-stu-id="3ce4a-112">id</span></span> |<span data-ttu-id="3ce4a-113">String</span><span class="sxs-lookup"><span data-stu-id="3ce4a-113">String</span></span> | <span data-ttu-id="3ce4a-114">A ID da organização conectada no gerenciamento de qualificação.</span><span class="sxs-lookup"><span data-stu-id="3ce4a-114">The ID of the connected organization in entitlement management.</span></span> |
| <span data-ttu-id="3ce4a-115">description</span><span class="sxs-lookup"><span data-stu-id="3ce4a-115">description</span></span> |<span data-ttu-id="3ce4a-116">String</span><span class="sxs-lookup"><span data-stu-id="3ce4a-116">String</span></span> | <span data-ttu-id="3ce4a-117">O nome da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="3ce4a-117">The name of the connected organization.</span></span> <span data-ttu-id="3ce4a-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce4a-118">Read only.</span></span> |
| <span data-ttu-id="3ce4a-119">IsBackup</span><span class="sxs-lookup"><span data-stu-id="3ce4a-119">isBackup</span></span> | <span data-ttu-id="3ce4a-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="3ce4a-120">Boolean</span></span> | <span data-ttu-id="3ce4a-121">Não usado no momento.</span><span class="sxs-lookup"><span data-stu-id="3ce4a-121">Not used at present.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3ce4a-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ce4a-122">JSON representation</span></span>

<span data-ttu-id="3ce4a-123">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="3ce4a-123">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectedOrganizationMembers",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "id": "string (identifier)",
  "description": "string",
  "isBackup": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectedOrganizationMembers complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


