---
title: Tipo de recurso onPremisesProvisioningError
description: Representa erros de sincronização de diretório para o grupo de usuários e recursos de contato ao sincronizar diretórios locais com o Azure Active Directory.
localization_priority: Normal
author: japere
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 2647e32653d26793b4f875bb47ce43e83a294c4a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133327"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="e7b58-103">Tipo de recurso onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="e7b58-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="e7b58-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7b58-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e7b58-105">Representa erros de sincronização de [](group.md) diretório para o [usuário,](user.md)grupo e [recursos orgContact](orgcontact.md) ao sincronizar diretórios locais com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e7b58-105">Represents directory synchronization errors for the [user](user.md), [group](group.md) and [orgContact](orgcontact.md) resources when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="e7b58-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e7b58-106">Properties</span></span>

| <span data-ttu-id="e7b58-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7b58-107">Property</span></span> | <span data-ttu-id="e7b58-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7b58-108">Type</span></span> | <span data-ttu-id="e7b58-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7b58-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e7b58-110">category</span><span class="sxs-lookup"><span data-stu-id="e7b58-110">category</span></span>|<span data-ttu-id="e7b58-111">String</span><span class="sxs-lookup"><span data-stu-id="e7b58-111">String</span></span>| <span data-ttu-id="e7b58-112">Categoria do erro de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="e7b58-112">Category of the provisioning error.</span></span> <span data-ttu-id="e7b58-113">Observação: Atualmente, há apenas um valor possível.</span><span class="sxs-lookup"><span data-stu-id="e7b58-113">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="e7b58-114">Valor possível: *PropertyConflict* – indica que um valor de propriedade não é exclusivo.</span><span class="sxs-lookup"><span data-stu-id="e7b58-114">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="e7b58-115">Outros objetos contêm o mesmo valor para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="e7b58-115">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="e7b58-116">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="e7b58-116">occurredDateTime</span></span>|<span data-ttu-id="e7b58-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7b58-117">DateTimeOffset</span></span>| <span data-ttu-id="e7b58-118">A data e a hora em que o erro ocorreu.</span><span class="sxs-lookup"><span data-stu-id="e7b58-118">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="e7b58-119">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="e7b58-119">propertyCausingError</span></span>|<span data-ttu-id="e7b58-120">String</span><span class="sxs-lookup"><span data-stu-id="e7b58-120">String</span></span>| <span data-ttu-id="e7b58-121">Nome da propriedade do diretório que está causando o erro.</span><span class="sxs-lookup"><span data-stu-id="e7b58-121">Name of the directory property causing the error.</span></span> <span data-ttu-id="e7b58-122">Valores atuais possíveis: *UserPrincipalName* ou *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="e7b58-122">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="e7b58-123">value</span><span class="sxs-lookup"><span data-stu-id="e7b58-123">value</span></span>|<span data-ttu-id="e7b58-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7b58-124">String</span></span>| <span data-ttu-id="e7b58-125">Valor da propriedade que está causando o erro.</span><span class="sxs-lookup"><span data-stu-id="e7b58-125">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e7b58-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e7b58-126">JSON representation</span></span>
<span data-ttu-id="e7b58-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e7b58-127">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

