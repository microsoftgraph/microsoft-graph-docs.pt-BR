---
title: tipo de recurso onPremisesProvisioningError
description: Representa erros de sincronização de diretório para o usuário, grupo ou entidades de contato organizacional ao sincronizar diretórios locais com o Azure Active Directory.
localization_priority: Normal
ms.openlocfilehash: e760493c388320c81d7773370a673aacc61fd3d5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345543"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="ce5fa-103">tipo de recurso onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="ce5fa-103">onPremisesProvisioningError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce5fa-104">Representa erros de sincronização de diretório para o [usuário](user.md), [grupo](group.md)ou entidades de [contato organizacional](orgcontact.md) ao sincronizar diretórios locais com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ce5fa-104">Represents directory synchronization errors for the [user](user.md), [group](group.md), or [organizational contact](orgcontact.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="ce5fa-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce5fa-105">Properties</span></span>

| <span data-ttu-id="ce5fa-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce5fa-106">Property</span></span> | <span data-ttu-id="ce5fa-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce5fa-107">Type</span></span> | <span data-ttu-id="ce5fa-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce5fa-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ce5fa-109">category</span><span class="sxs-lookup"><span data-stu-id="ce5fa-109">category</span></span>|<span data-ttu-id="ce5fa-110">String</span><span class="sxs-lookup"><span data-stu-id="ce5fa-110">String</span></span>| <span data-ttu-id="ce5fa-111">Categoria do erro de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="ce5fa-111">Category of the provisioning error.</span></span> <span data-ttu-id="ce5fa-112">Observação: no momento, há apenas um valor possível.</span><span class="sxs-lookup"><span data-stu-id="ce5fa-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="ce5fa-113">Valor possível: *PropertyConflict* -indica que um valor de propriedade não é exclusivo.</span><span class="sxs-lookup"><span data-stu-id="ce5fa-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="ce5fa-114">Outros objetos contêm o mesmo valor para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="ce5fa-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="ce5fa-115">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="ce5fa-115">occurredDateTime</span></span>|<span data-ttu-id="ce5fa-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce5fa-116">DateTimeOffset</span></span>| <span data-ttu-id="ce5fa-117">A data e a hora em que o erro ocorreu.</span><span class="sxs-lookup"><span data-stu-id="ce5fa-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="ce5fa-118">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="ce5fa-118">propertyCausingError</span></span>|<span data-ttu-id="ce5fa-119">String</span><span class="sxs-lookup"><span data-stu-id="ce5fa-119">String</span></span>| <span data-ttu-id="ce5fa-120">Nome da propriedade de diretório que está causando o erro.</span><span class="sxs-lookup"><span data-stu-id="ce5fa-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="ce5fa-121">Valores possíveis atuais: *userPrincipalName* ou *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="ce5fa-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="ce5fa-122">value</span><span class="sxs-lookup"><span data-stu-id="ce5fa-122">value</span></span>|<span data-ttu-id="ce5fa-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce5fa-123">String</span></span>| <span data-ttu-id="ce5fa-124">Valor da propriedade causando o erro.</span><span class="sxs-lookup"><span data-stu-id="ce5fa-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ce5fa-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce5fa-125">JSON representation</span></span>
<span data-ttu-id="ce5fa-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce5fa-126">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
