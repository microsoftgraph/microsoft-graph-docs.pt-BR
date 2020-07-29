---
title: tipo complexo connectedOrganizationMembers
description: O tipo connectedOrganizationMembers identifica uma coleção de usuários no locatário que serão permitidos como solicitante, Aprovador ou revisor.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7eddc19d3d802174ca015877ec362ec742f2e791
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509795"
---
# <a name="connectedorganizationmembers-complex-type"></a><span data-ttu-id="e906c-103">tipo complexo connectedOrganizationMembers</span><span class="sxs-lookup"><span data-stu-id="e906c-103">connectedOrganizationMembers complex type</span></span>

<span data-ttu-id="e906c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e906c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e906c-105">Usado nas configurações de solicitação de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e906c-105">Used in the request settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="e906c-106">O `@odata.type` valor `#microsoft.graph.connectedOrganizationMembers` indica que esse tipo identifica uma coleção de usuários, os que estão associados a uma [organização conectada](connectedorganization.md), que terá permissão para solicitar um pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="e906c-106">The `@odata.type` value `#microsoft.graph.connectedOrganizationMembers` indicates that this type identifies a collection of users, those who are associated with a [connected organization](connectedorganization.md), who will be allowed to request an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="e906c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e906c-107">Properties</span></span>

<span data-ttu-id="e906c-108">Este tipo tem as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="e906c-108">This type has the following properties:</span></span>

| <span data-ttu-id="e906c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e906c-109">Property</span></span>                     | <span data-ttu-id="e906c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e906c-110">Type</span></span>                      | <span data-ttu-id="e906c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e906c-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="e906c-112">id</span><span class="sxs-lookup"><span data-stu-id="e906c-112">id</span></span> |<span data-ttu-id="e906c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e906c-113">String</span></span> | <span data-ttu-id="e906c-114">A ID da organização conectada no gerenciamento de qualificação.</span><span class="sxs-lookup"><span data-stu-id="e906c-114">The ID of the connected organization in entitlement management.</span></span> |
| <span data-ttu-id="e906c-115">description</span><span class="sxs-lookup"><span data-stu-id="e906c-115">description</span></span> |<span data-ttu-id="e906c-116">String</span><span class="sxs-lookup"><span data-stu-id="e906c-116">String</span></span> | <span data-ttu-id="e906c-117">O nome da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="e906c-117">The name of the connected organization.</span></span> <span data-ttu-id="e906c-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e906c-118">Read only.</span></span> |
| <span data-ttu-id="e906c-119">IsBackup</span><span class="sxs-lookup"><span data-stu-id="e906c-119">isBackup</span></span> | <span data-ttu-id="e906c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="e906c-120">Boolean</span></span> | <span data-ttu-id="e906c-121">Não usado no momento.</span><span class="sxs-lookup"><span data-stu-id="e906c-121">Not used at present.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e906c-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e906c-122">JSON representation</span></span>

<span data-ttu-id="e906c-123">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="e906c-123">The following is a JSON representation of the type.</span></span>

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
