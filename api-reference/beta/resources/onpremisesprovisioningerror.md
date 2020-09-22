---
title: tipo de recurso onPremisesProvisioningError
description: Representa erros de sincronização de diretório para o usuário, grupo ou entidades de contato organizacional ao sincronizar diretórios locais com o Azure Active Directory.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: japere
ms.openlocfilehash: ac6ae129374ab33e44a1f3274e8be378b90eb4e1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052583"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="0a8ce-103">tipo de recurso onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="0a8ce-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="0a8ce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a8ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a8ce-105">Representa erros de sincronização de diretório para o [usuário](user.md), [grupo](group.md)ou entidades de [contato organizacional](orgcontact.md) ao sincronizar diretórios locais com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0a8ce-105">Represents directory synchronization errors for the [user](user.md), [group](group.md), or [organizational contact](orgcontact.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="0a8ce-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0a8ce-106">Properties</span></span>

| <span data-ttu-id="0a8ce-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a8ce-107">Property</span></span> | <span data-ttu-id="0a8ce-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a8ce-108">Type</span></span> | <span data-ttu-id="0a8ce-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a8ce-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0a8ce-110">category</span><span class="sxs-lookup"><span data-stu-id="0a8ce-110">category</span></span>|<span data-ttu-id="0a8ce-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a8ce-111">String</span></span>| <span data-ttu-id="0a8ce-112">Categoria do erro de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="0a8ce-112">Category of the provisioning error.</span></span> <span data-ttu-id="0a8ce-113">Observação: no momento, há apenas um valor possível.</span><span class="sxs-lookup"><span data-stu-id="0a8ce-113">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="0a8ce-114">Valor possível: *PropertyConflict* -indica que um valor de propriedade não é exclusivo.</span><span class="sxs-lookup"><span data-stu-id="0a8ce-114">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="0a8ce-115">Outros objetos contêm o mesmo valor para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="0a8ce-115">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="0a8ce-116">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="0a8ce-116">occurredDateTime</span></span>|<span data-ttu-id="0a8ce-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a8ce-117">DateTimeOffset</span></span>| <span data-ttu-id="0a8ce-118">A data e a hora em que o erro ocorreu.</span><span class="sxs-lookup"><span data-stu-id="0a8ce-118">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="0a8ce-119">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="0a8ce-119">propertyCausingError</span></span>|<span data-ttu-id="0a8ce-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a8ce-120">String</span></span>| <span data-ttu-id="0a8ce-121">Nome da propriedade de diretório que está causando o erro.</span><span class="sxs-lookup"><span data-stu-id="0a8ce-121">Name of the directory property causing the error.</span></span> <span data-ttu-id="0a8ce-122">Valores possíveis atuais: *userPrincipalName* ou *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="0a8ce-122">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="0a8ce-123">value</span><span class="sxs-lookup"><span data-stu-id="0a8ce-123">value</span></span>|<span data-ttu-id="0a8ce-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a8ce-124">String</span></span>| <span data-ttu-id="0a8ce-125">Valor da propriedade causando o erro.</span><span class="sxs-lookup"><span data-stu-id="0a8ce-125">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0a8ce-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0a8ce-126">JSON representation</span></span>
<span data-ttu-id="0a8ce-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0a8ce-127">Here is a JSON representation of the resource.</span></span>

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


