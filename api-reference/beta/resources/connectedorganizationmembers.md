---
title: tipo complexo connectedOrganizationMembers
description: O tipo connectedOrganizationMembers identifica uma coleção de usuários no locatário que serão permitidos como solicitante, Aprovador ou revisor.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f2a3b55e3fab41f0fe08fcf844a6d143b12d7146
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331360"
---
# <a name="connectedorganizationmembers-complex-type"></a><span data-ttu-id="51cd5-103">tipo complexo connectedOrganizationMembers</span><span class="sxs-lookup"><span data-stu-id="51cd5-103">connectedOrganizationMembers complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51cd5-104">Usado nas configurações de solicitação de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="51cd5-104">Used in the request settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="51cd5-105">O `@odata.type` valor `#microsoft.graph.connectedOrganizationMembers` indica que esse tipo identifica uma coleção de usuários, os que estão associados a uma organização conectada, que terá permissão para solicitar um pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="51cd5-105">The `@odata.type` value `#microsoft.graph.connectedOrganizationMembers` indicates that this type identifies a collection of users, those who are associated with a connected organization, who will be allowed to request an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="51cd5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51cd5-106">Properties</span></span>

<span data-ttu-id="51cd5-107">Este tipo tem as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="51cd5-107">This type has the following properties:</span></span>

| <span data-ttu-id="51cd5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51cd5-108">Property</span></span>                     | <span data-ttu-id="51cd5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="51cd5-109">Type</span></span>                      | <span data-ttu-id="51cd5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="51cd5-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="51cd5-111">id</span><span class="sxs-lookup"><span data-stu-id="51cd5-111">id</span></span> |<span data-ttu-id="51cd5-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51cd5-112">String</span></span> | <span data-ttu-id="51cd5-113">A ID da organização conectada no gerenciamento de qualificação.</span><span class="sxs-lookup"><span data-stu-id="51cd5-113">The ID of the connected organization in entitlement management.</span></span> |
| <span data-ttu-id="51cd5-114">descrição</span><span class="sxs-lookup"><span data-stu-id="51cd5-114">description</span></span> |<span data-ttu-id="51cd5-115">String</span><span class="sxs-lookup"><span data-stu-id="51cd5-115">String</span></span> | <span data-ttu-id="51cd5-116">O nome da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="51cd5-116">The name of the connected organization.</span></span> <span data-ttu-id="51cd5-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51cd5-117">Read only.</span></span> |
| <span data-ttu-id="51cd5-118">IsBackup</span><span class="sxs-lookup"><span data-stu-id="51cd5-118">isBackup</span></span> | <span data-ttu-id="51cd5-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="51cd5-119">Boolean</span></span> | <span data-ttu-id="51cd5-120">Não usado no momento.</span><span class="sxs-lookup"><span data-stu-id="51cd5-120">Not used at present.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="51cd5-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51cd5-121">JSON representation</span></span>

<span data-ttu-id="51cd5-122">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="51cd5-122">The following is a JSON representation of the type.</span></span>

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
