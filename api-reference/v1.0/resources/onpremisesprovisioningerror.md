---
title: tipo de recurso onPremisesProvisioningError
description: Representa erros de sincronização de diretório para o grupo de usuários e recursos de contato durante a sincronização de diretórios locais com o Azure Active Directory.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ccbb10bdf5dba14a01a572198dbdbbafb2534eb7
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621649"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="ce436-103">tipo de recurso onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="ce436-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="ce436-104">Representa erros de sincronização de diretório para os recursos de [usuário](user.md), [grupo](group.md) e [orgContact](orgcontact.md) ao sincronizar diretórios locais com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ce436-104">Represents directory synchronization errors for the [user](user.md), [group](group.md) and [orgContact](orgcontact.md) resources when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="ce436-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce436-105">Properties</span></span>

| <span data-ttu-id="ce436-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce436-106">Property</span></span> | <span data-ttu-id="ce436-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce436-107">Type</span></span> | <span data-ttu-id="ce436-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce436-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ce436-109">category</span><span class="sxs-lookup"><span data-stu-id="ce436-109">category</span></span>|<span data-ttu-id="ce436-110">String</span><span class="sxs-lookup"><span data-stu-id="ce436-110">String</span></span>| <span data-ttu-id="ce436-111">Categoria do erro de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="ce436-111">Category of the provisioning error.</span></span> <span data-ttu-id="ce436-112">Observação: no momento, há apenas um valor possível.</span><span class="sxs-lookup"><span data-stu-id="ce436-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="ce436-113">Valor possível: *PropertyConflict* -indica que um valor de propriedade não é exclusivo.</span><span class="sxs-lookup"><span data-stu-id="ce436-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="ce436-114">Outros objetos contêm o mesmo valor para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="ce436-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="ce436-115">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="ce436-115">occurredDateTime</span></span>|<span data-ttu-id="ce436-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce436-116">DateTimeOffset</span></span>| <span data-ttu-id="ce436-117">A data e a hora em que o erro ocorreu.</span><span class="sxs-lookup"><span data-stu-id="ce436-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="ce436-118">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="ce436-118">propertyCausingError</span></span>|<span data-ttu-id="ce436-119">String</span><span class="sxs-lookup"><span data-stu-id="ce436-119">String</span></span>| <span data-ttu-id="ce436-120">Nome da propriedade de diretório que está causando o erro.</span><span class="sxs-lookup"><span data-stu-id="ce436-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="ce436-121">Valores possíveis atuais: *userPrincipalName* ou *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="ce436-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="ce436-122">value</span><span class="sxs-lookup"><span data-stu-id="ce436-122">value</span></span>|<span data-ttu-id="ce436-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce436-123">String</span></span>| <span data-ttu-id="ce436-124">Valor da propriedade causando o erro.</span><span class="sxs-lookup"><span data-stu-id="ce436-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ce436-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce436-125">JSON representation</span></span>
<span data-ttu-id="ce436-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce436-126">Here is a JSON representation of the resource.</span></span>

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
