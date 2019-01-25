---
title: tipo de recurso de onPremisesProvisioningError
description: Representa os erros de sincronização de diretório para o usuário, grupo ou organizacionais entidades visita quando a sincronização local diretórios no Windows Azure Active Directory.
localization_priority: Normal
ms.openlocfilehash: 7e4d51ea3bde6158256c607027b3e56236a8151c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512728"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="8e1d2-103">tipo de recurso de onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="8e1d2-103">onPremisesProvisioningError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e1d2-104">Representa os erros de sincronização de diretório para as entidades de [usuário](user.md), [grupo](group.md)ou [contato organizacional](orgcontact.md) quando a sincronização local diretórios no Windows Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8e1d2-104">Represents directory synchronization errors for the [user](user.md), [group](group.md), or [organizational contact](orgcontact.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="8e1d2-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e1d2-105">Properties</span></span>

| <span data-ttu-id="8e1d2-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e1d2-106">Property</span></span> | <span data-ttu-id="8e1d2-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e1d2-107">Type</span></span> | <span data-ttu-id="8e1d2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e1d2-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8e1d2-109">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="8e1d2-109">category</span></span>|<span data-ttu-id="8e1d2-110">String</span><span class="sxs-lookup"><span data-stu-id="8e1d2-110">String</span></span>| <span data-ttu-id="8e1d2-111">Categoria do erro provisionamento.</span><span class="sxs-lookup"><span data-stu-id="8e1d2-111">Category of the provisioning error.</span></span> <span data-ttu-id="8e1d2-112">Observação: No momento, há apenas um valor possível.</span><span class="sxs-lookup"><span data-stu-id="8e1d2-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="8e1d2-113">Valores possíveis: *PropertyConflict* - indica um valor de propriedade não é exclusivo.</span><span class="sxs-lookup"><span data-stu-id="8e1d2-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="8e1d2-114">Outros objetos contenham o mesmo valor da propriedade.</span><span class="sxs-lookup"><span data-stu-id="8e1d2-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="8e1d2-115">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="8e1d2-115">occurredDateTime</span></span>|<span data-ttu-id="8e1d2-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e1d2-116">DateTimeOffset</span></span>| <span data-ttu-id="8e1d2-117">A data e hora em que o erro ocorreu.</span><span class="sxs-lookup"><span data-stu-id="8e1d2-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="8e1d2-118">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="8e1d2-118">propertyCausingError</span></span>|<span data-ttu-id="8e1d2-119">String</span><span class="sxs-lookup"><span data-stu-id="8e1d2-119">String</span></span>| <span data-ttu-id="8e1d2-120">Nome da propriedade diretório que causou o erro.</span><span class="sxs-lookup"><span data-stu-id="8e1d2-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="8e1d2-121">Valores possíveis atuais: *UserPrincipalName* ou *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="8e1d2-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="8e1d2-122">valor</span><span class="sxs-lookup"><span data-stu-id="8e1d2-122">value</span></span>|<span data-ttu-id="8e1d2-123">String</span><span class="sxs-lookup"><span data-stu-id="8e1d2-123">String</span></span>| <span data-ttu-id="8e1d2-124">Valor da propriedade que causou o erro.</span><span class="sxs-lookup"><span data-stu-id="8e1d2-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8e1d2-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e1d2-125">JSON representation</span></span>
<span data-ttu-id="8e1d2-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e1d2-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisesprovisioningerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
