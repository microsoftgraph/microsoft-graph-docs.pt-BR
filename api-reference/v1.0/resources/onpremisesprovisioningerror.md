---
title: tipo de recurso onPremisesProvisioningError
description: Representa erros de sincronização de diretório para o grupo de usuários e recursos de contato durante a sincronização de diretórios locais com o Azure Active Directory.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 719bb525fad934bb92f44fb427d1214bf288ec46
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059086"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="c4d81-103">tipo de recurso onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="c4d81-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="c4d81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4d81-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c4d81-105">Representa erros de sincronização de diretório para os recursos de [usuário](user.md), [grupo](group.md) e [orgContact](orgcontact.md) ao sincronizar diretórios locais com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c4d81-105">Represents directory synchronization errors for the [user](user.md), [group](group.md) and [orgContact](orgcontact.md) resources when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="c4d81-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c4d81-106">Properties</span></span>

| <span data-ttu-id="c4d81-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4d81-107">Property</span></span> | <span data-ttu-id="c4d81-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4d81-108">Type</span></span> | <span data-ttu-id="c4d81-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4d81-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c4d81-110">category</span><span class="sxs-lookup"><span data-stu-id="c4d81-110">category</span></span>|<span data-ttu-id="c4d81-111">String</span><span class="sxs-lookup"><span data-stu-id="c4d81-111">String</span></span>| <span data-ttu-id="c4d81-112">Categoria do erro de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="c4d81-112">Category of the provisioning error.</span></span> <span data-ttu-id="c4d81-113">Observação: no momento, há apenas um valor possível.</span><span class="sxs-lookup"><span data-stu-id="c4d81-113">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="c4d81-114">Valor possível: *PropertyConflict* -indica que um valor de propriedade não é exclusivo.</span><span class="sxs-lookup"><span data-stu-id="c4d81-114">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="c4d81-115">Outros objetos contêm o mesmo valor para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="c4d81-115">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="c4d81-116">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="c4d81-116">occurredDateTime</span></span>|<span data-ttu-id="c4d81-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4d81-117">DateTimeOffset</span></span>| <span data-ttu-id="c4d81-118">A data e a hora em que o erro ocorreu.</span><span class="sxs-lookup"><span data-stu-id="c4d81-118">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="c4d81-119">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="c4d81-119">propertyCausingError</span></span>|<span data-ttu-id="c4d81-120">String</span><span class="sxs-lookup"><span data-stu-id="c4d81-120">String</span></span>| <span data-ttu-id="c4d81-121">Nome da propriedade de diretório que está causando o erro.</span><span class="sxs-lookup"><span data-stu-id="c4d81-121">Name of the directory property causing the error.</span></span> <span data-ttu-id="c4d81-122">Valores possíveis atuais: *userPrincipalName* ou *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="c4d81-122">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="c4d81-123">value</span><span class="sxs-lookup"><span data-stu-id="c4d81-123">value</span></span>|<span data-ttu-id="c4d81-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4d81-124">String</span></span>| <span data-ttu-id="c4d81-125">Valor da propriedade causando o erro.</span><span class="sxs-lookup"><span data-stu-id="c4d81-125">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c4d81-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c4d81-126">JSON representation</span></span>
<span data-ttu-id="c4d81-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c4d81-127">Here is a JSON representation of the resource.</span></span>

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

