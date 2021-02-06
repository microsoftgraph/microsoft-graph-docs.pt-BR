---
title: Tipo de recurso onPremisesProvisioningError
description: Representa erros de sincronização de diretório para as entidades de usuário, grupo ou contato organizacional ao sincronizar diretórios locais com o Azure Active Directory.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: japere
ms.openlocfilehash: e4e3469ae371568ac9010d1d3879f68c92340460
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133975"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="a195e-103">Tipo de recurso onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="a195e-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="a195e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a195e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a195e-105">Representa erros de sincronização de [](group.md)diretório [](orgcontact.md) para o [usuário,](user.md)grupo ou entidades de contato organizacional ao sincronizar diretórios locais com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a195e-105">Represents directory synchronization errors for the [user](user.md), [group](group.md), or [organizational contact](orgcontact.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="a195e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a195e-106">Properties</span></span>

| <span data-ttu-id="a195e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a195e-107">Property</span></span> | <span data-ttu-id="a195e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a195e-108">Type</span></span> | <span data-ttu-id="a195e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a195e-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a195e-110">category</span><span class="sxs-lookup"><span data-stu-id="a195e-110">category</span></span>|<span data-ttu-id="a195e-111">String</span><span class="sxs-lookup"><span data-stu-id="a195e-111">String</span></span>| <span data-ttu-id="a195e-112">Categoria do erro de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="a195e-112">Category of the provisioning error.</span></span> <span data-ttu-id="a195e-113">Observação: Atualmente, há apenas um valor possível.</span><span class="sxs-lookup"><span data-stu-id="a195e-113">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="a195e-114">Valor possível: *PropertyConflict* – indica que um valor de propriedade não é exclusivo.</span><span class="sxs-lookup"><span data-stu-id="a195e-114">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="a195e-115">Outros objetos contêm o mesmo valor para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="a195e-115">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="a195e-116">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="a195e-116">occurredDateTime</span></span>|<span data-ttu-id="a195e-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a195e-117">DateTimeOffset</span></span>| <span data-ttu-id="a195e-118">A data e a hora em que o erro ocorreu.</span><span class="sxs-lookup"><span data-stu-id="a195e-118">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="a195e-119">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="a195e-119">propertyCausingError</span></span>|<span data-ttu-id="a195e-120">String</span><span class="sxs-lookup"><span data-stu-id="a195e-120">String</span></span>| <span data-ttu-id="a195e-121">Nome da propriedade de diretório que está causando o erro.</span><span class="sxs-lookup"><span data-stu-id="a195e-121">Name of the directory property causing the error.</span></span> <span data-ttu-id="a195e-122">Valores atuais possíveis: *UserPrincipalName* ou *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="a195e-122">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="a195e-123">value</span><span class="sxs-lookup"><span data-stu-id="a195e-123">value</span></span>|<span data-ttu-id="a195e-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a195e-124">String</span></span>| <span data-ttu-id="a195e-125">Valor da propriedade que está causando o erro.</span><span class="sxs-lookup"><span data-stu-id="a195e-125">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a195e-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a195e-126">JSON representation</span></span>
<span data-ttu-id="a195e-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a195e-127">Here is a JSON representation of the resource.</span></span>

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


