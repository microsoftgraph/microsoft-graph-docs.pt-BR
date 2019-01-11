---
title: tipo de recurso de onPremisesProvisioningError
description: Representa os erros de sincronização de diretório para as entidades de usuário e grupo durante a sincronização de diretórios no local com o Windows Azure Active Directory.
localization_priority: Normal
ms.openlocfilehash: c8989a78dfb60a6c7c25a66a9f1e619dcbdca15d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830664"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="de283-103">tipo de recurso de onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="de283-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="de283-104">Representa os erros de sincronização de diretório para as entidades de [usuário](user.md) e [grupo](group.md) quando a sincronização local diretórios no Windows Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="de283-104">Represents directory synchronization errors for the [user](user.md) and [group](group.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="de283-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de283-105">Properties</span></span>

| <span data-ttu-id="de283-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de283-106">Property</span></span> | <span data-ttu-id="de283-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="de283-107">Type</span></span> | <span data-ttu-id="de283-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="de283-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="de283-109">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="de283-109">category</span></span>|<span data-ttu-id="de283-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de283-110">String</span></span>| <span data-ttu-id="de283-111">Categoria do erro provisionamento.</span><span class="sxs-lookup"><span data-stu-id="de283-111">Category of the provisioning error.</span></span> <span data-ttu-id="de283-112">Observação: No momento, há apenas um valor possível.</span><span class="sxs-lookup"><span data-stu-id="de283-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="de283-113">Valores possíveis: *PropertyConflict* - indica um valor de propriedade não é exclusivo.</span><span class="sxs-lookup"><span data-stu-id="de283-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="de283-114">Outros objetos contenham o mesmo valor da propriedade.</span><span class="sxs-lookup"><span data-stu-id="de283-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="de283-115">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="de283-115">occurredDateTime</span></span>|<span data-ttu-id="de283-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de283-116">DateTimeOffset</span></span>| <span data-ttu-id="de283-117">A data e hora em que o erro ocorreu.</span><span class="sxs-lookup"><span data-stu-id="de283-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="de283-118">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="de283-118">propertyCausingError</span></span>|<span data-ttu-id="de283-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de283-119">String</span></span>| <span data-ttu-id="de283-120">Nome da propriedade diretório que causou o erro.</span><span class="sxs-lookup"><span data-stu-id="de283-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="de283-121">Valores possíveis atuais: *UserPrincipalName* ou *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="de283-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="de283-122">valor</span><span class="sxs-lookup"><span data-stu-id="de283-122">value</span></span>|<span data-ttu-id="de283-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de283-123">String</span></span>| <span data-ttu-id="de283-124">Valor da propriedade que causou o erro.</span><span class="sxs-lookup"><span data-stu-id="de283-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="de283-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de283-125">JSON representation</span></span>
<span data-ttu-id="de283-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="de283-126">Here is a JSON representation of the resource.</span></span>

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
