---
title: tipo de recurso onPremisesProvisioningError
description: Representa erros de sincronização de diretório para o usuário, grupo ou entidades de contato organizacional ao sincronizar diretórios locais com o Azure Active Directory.
localization_priority: Normal
ms.openlocfilehash: 7e4d51ea3bde6158256c607027b3e56236a8151c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568847"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="26e61-103">tipo de recurso onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="26e61-103">onPremisesProvisioningError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26e61-104">Representa erros de sincronização de diretório para o [usuário](user.md), [grupo](group.md)ou entidades de [contato organizacional](orgcontact.md) ao sincronizar diretórios locais com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="26e61-104">Represents directory synchronization errors for the [user](user.md), [group](group.md), or [organizational contact](orgcontact.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="26e61-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="26e61-105">Properties</span></span>

| <span data-ttu-id="26e61-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26e61-106">Property</span></span> | <span data-ttu-id="26e61-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="26e61-107">Type</span></span> | <span data-ttu-id="26e61-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="26e61-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="26e61-109">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="26e61-109">category</span></span>|<span data-ttu-id="26e61-110">String</span><span class="sxs-lookup"><span data-stu-id="26e61-110">String</span></span>| <span data-ttu-id="26e61-111">Categoria do erro de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="26e61-111">Category of the provisioning error.</span></span> <span data-ttu-id="26e61-112">Observação: no momento, há apenas um valor possível.</span><span class="sxs-lookup"><span data-stu-id="26e61-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="26e61-113">Valor possível: *PropertyConflict* -indica que um valor de propriedade não é exclusivo.</span><span class="sxs-lookup"><span data-stu-id="26e61-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="26e61-114">Outros objetos contêm o mesmo valor para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="26e61-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="26e61-115">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="26e61-115">occurredDateTime</span></span>|<span data-ttu-id="26e61-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26e61-116">DateTimeOffset</span></span>| <span data-ttu-id="26e61-117">A data e a hora em que o erro ocorreu.</span><span class="sxs-lookup"><span data-stu-id="26e61-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="26e61-118">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="26e61-118">propertyCausingError</span></span>|<span data-ttu-id="26e61-119">String</span><span class="sxs-lookup"><span data-stu-id="26e61-119">String</span></span>| <span data-ttu-id="26e61-120">Nome da propriedade de diretório que está causando o erro.</span><span class="sxs-lookup"><span data-stu-id="26e61-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="26e61-121">Valores possíveis atuais: *userPrincipalName* ou *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="26e61-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="26e61-122">value</span><span class="sxs-lookup"><span data-stu-id="26e61-122">value</span></span>|<span data-ttu-id="26e61-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26e61-123">String</span></span>| <span data-ttu-id="26e61-124">Valor da propriedade causando o erro.</span><span class="sxs-lookup"><span data-stu-id="26e61-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="26e61-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="26e61-125">JSON representation</span></span>
<span data-ttu-id="26e61-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="26e61-126">Here is a JSON representation of the resource.</span></span>

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
