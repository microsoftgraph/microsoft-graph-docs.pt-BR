---
title: tipo de recurso de governancePermission
description: 'Representa a permissão de acesso que tenha um governanceSubject um governanceResource específico.  '
localization_priority: Normal
ms.openlocfilehash: 255cd4c25a957a40e5e5ac765ed446f516c51607
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643780"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="1fd1c-103">tipo de recurso de governancePermission</span><span class="sxs-lookup"><span data-stu-id="1fd1c-103">governancePermission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fd1c-104">Representa a permissão de acesso que um [governanceSubject](../resources/governancesubject.md) tem um específicos [governanceResource](../resources/governanceresource.md).</span><span class="sxs-lookup"><span data-stu-id="1fd1c-104">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="1fd1c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1fd1c-105">Properties</span></span>
| <span data-ttu-id="1fd1c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1fd1c-106">Property</span></span>     | <span data-ttu-id="1fd1c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fd1c-107">Type</span></span>   |<span data-ttu-id="1fd1c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fd1c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1fd1c-109">accessLevel</span><span class="sxs-lookup"><span data-stu-id="1fd1c-109">accessLevel</span></span>|<span data-ttu-id="1fd1c-110">String</span><span class="sxs-lookup"><span data-stu-id="1fd1c-110">String</span></span>|<span data-ttu-id="1fd1c-111">O nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="1fd1c-111">The access level.</span></span> <span data-ttu-id="1fd1c-112">Valores válidos: ``None``, ``UserRead``, ``AdminRead``, e ``AdminReadWrite``.</span><span class="sxs-lookup"><span data-stu-id="1fd1c-112">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="1fd1c-113">isActive</span><span class="sxs-lookup"><span data-stu-id="1fd1c-113">isActive</span></span>|<span data-ttu-id="1fd1c-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="1fd1c-114">Boolean</span></span>|<span data-ttu-id="1fd1c-115">Indique se o solicitante tem qualquer atribuição de função ativa para o nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="1fd1c-115">Indicate if the the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="1fd1c-116">isEligible</span><span class="sxs-lookup"><span data-stu-id="1fd1c-116">isEligible</span></span>|<span data-ttu-id="1fd1c-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="1fd1c-117">Boolean</span></span>|<span data-ttu-id="1fd1c-118">Indica se o solicitante tem qualquer atribuição de função elegíveis para o nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="1fd1c-118">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1fd1c-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1fd1c-119">JSON representation</span></span>

<span data-ttu-id="1fd1c-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1fd1c-120">Here is a JSON representation of the resource.</span></span>

```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancepermission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
