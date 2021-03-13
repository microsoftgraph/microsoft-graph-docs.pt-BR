---
title: tipo complexo connectedOrganizationMembers
description: O tipo connectedOrganizationMembers identifica uma coleção de usuários no locatário que serão permitidos como solicitante, aprovador ou revisor.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 725926bc39583bda653294f0cc917ea7d2f08a45
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761811"
---
# <a name="connectedorganizationmembers-complex-type"></a><span data-ttu-id="06cf9-103">tipo complexo connectedOrganizationMembers</span><span class="sxs-lookup"><span data-stu-id="06cf9-103">connectedOrganizationMembers complex type</span></span>

<span data-ttu-id="06cf9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06cf9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06cf9-105">Usado nas configurações de solicitação de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="06cf9-105">Used in the request settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="06cf9-106">O valor indica que esse tipo identifica uma coleção de usuários, aqueles associados a uma organização conectada, que terão permissão para solicitar `@odata.type` `#microsoft.graph.connectedOrganizationMembers` um pacote de acesso. [](connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="06cf9-106">The `@odata.type` value `#microsoft.graph.connectedOrganizationMembers` indicates that this type identifies a collection of users, those who are associated with a [connected organization](connectedorganization.md), who will be allowed to request an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="06cf9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="06cf9-107">Properties</span></span>

<span data-ttu-id="06cf9-108">Esse tipo tem as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="06cf9-108">This type has the following properties:</span></span>

| <span data-ttu-id="06cf9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06cf9-109">Property</span></span>                     | <span data-ttu-id="06cf9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="06cf9-110">Type</span></span>                      | <span data-ttu-id="06cf9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="06cf9-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="06cf9-112">id</span><span class="sxs-lookup"><span data-stu-id="06cf9-112">id</span></span> |<span data-ttu-id="06cf9-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06cf9-113">String</span></span> | <span data-ttu-id="06cf9-114">A ID da organização conectada no gerenciamento de direitos.</span><span class="sxs-lookup"><span data-stu-id="06cf9-114">The ID of the connected organization in entitlement management.</span></span> |
| <span data-ttu-id="06cf9-115">descrição</span><span class="sxs-lookup"><span data-stu-id="06cf9-115">description</span></span> |<span data-ttu-id="06cf9-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06cf9-116">String</span></span> | <span data-ttu-id="06cf9-117">O nome da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="06cf9-117">The name of the connected organization.</span></span> <span data-ttu-id="06cf9-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="06cf9-118">Read only.</span></span> |
| <span data-ttu-id="06cf9-119">isBackup</span><span class="sxs-lookup"><span data-stu-id="06cf9-119">isBackup</span></span> | <span data-ttu-id="06cf9-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="06cf9-120">Boolean</span></span> | <span data-ttu-id="06cf9-121">Não é usado no momento.</span><span class="sxs-lookup"><span data-stu-id="06cf9-121">Not used at present.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="06cf9-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="06cf9-122">JSON representation</span></span>

<span data-ttu-id="06cf9-123">A seguir está uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="06cf9-123">The following is a JSON representation of the type.</span></span>

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


