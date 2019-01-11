---
title: tipo de recurso de deviceDetail
description: Indica os detalhes do dispositivo associados a um dispositivo usado para assinar. Inclui informações como o navegador do dispositivo e informações do sistema operacional, se o dispositivo for Azure AD gerenciado.
localization_priority: Normal
ms.openlocfilehash: ca4679a8c484b6dc5b36ef39d3d6d039537cbdbb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884837"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="744c0-104">tipo de recurso de deviceDetail</span><span class="sxs-lookup"><span data-stu-id="744c0-104">deviceDetail resource type</span></span>
<span data-ttu-id="744c0-105">Indica os detalhes do dispositivo associados a um dispositivo usado para assinar.</span><span class="sxs-lookup"><span data-stu-id="744c0-105">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="744c0-106">Inclui informações como o navegador do dispositivo e informações do sistema operacional, se o dispositivo for Azure AD gerenciado.</span><span class="sxs-lookup"><span data-stu-id="744c0-106">Includes information like device browser and  OS info, if device is Azure AD managed.</span></span>



## <a name="properties"></a><span data-ttu-id="744c0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="744c0-107">Properties</span></span>
| <span data-ttu-id="744c0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="744c0-108">Property</span></span>     | <span data-ttu-id="744c0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="744c0-109">Type</span></span>   |<span data-ttu-id="744c0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="744c0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="744c0-111">Navegador</span><span class="sxs-lookup"><span data-stu-id="744c0-111">browser</span></span>|<span data-ttu-id="744c0-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="744c0-112">String</span></span>|<span data-ttu-id="744c0-113">Indica as informações do navegador dos usados para entrar no serviço.</span><span class="sxs-lookup"><span data-stu-id="744c0-113">Indicates the browser information of the used for signing-in.</span></span>|
|<span data-ttu-id="744c0-114">deviceId</span><span class="sxs-lookup"><span data-stu-id="744c0-114">deviceId</span></span>|<span data-ttu-id="744c0-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="744c0-115">String</span></span>|<span data-ttu-id="744c0-116">Refere-se o UniqueID do dispositivo usado para entrar no serviço.</span><span class="sxs-lookup"><span data-stu-id="744c0-116">Refers to the UniqueID of the device used for signing-in.</span></span>|
|<span data-ttu-id="744c0-117">displayName</span><span class="sxs-lookup"><span data-stu-id="744c0-117">displayName</span></span>|<span data-ttu-id="744c0-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="744c0-118">String</span></span>|<span data-ttu-id="744c0-119">Refere-se com o nome do dispositivo usado para entrar no serviço.</span><span class="sxs-lookup"><span data-stu-id="744c0-119">Refers to the name of the device used for signing-in.</span></span>|
|<span data-ttu-id="744c0-120">isCompliant</span><span class="sxs-lookup"><span data-stu-id="744c0-120">isCompliant</span></span>|<span data-ttu-id="744c0-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="744c0-121">Boolean</span></span>|<span data-ttu-id="744c0-122">Indica se o dispositivo é compatível com ou não.</span><span class="sxs-lookup"><span data-stu-id="744c0-122">Indicates whether the device is compliant or not.</span></span>|
|<span data-ttu-id="744c0-123">isManaged</span><span class="sxs-lookup"><span data-stu-id="744c0-123">isManaged</span></span>|<span data-ttu-id="744c0-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="744c0-124">Boolean</span></span>|<span data-ttu-id="744c0-125">Indica se o dispositivo é gerenciado ou não.</span><span class="sxs-lookup"><span data-stu-id="744c0-125">Indicates if the device is managed or not.</span></span>|
|<span data-ttu-id="744c0-126">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="744c0-126">operatingSystem</span></span>|<span data-ttu-id="744c0-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="744c0-127">String</span></span>|<span data-ttu-id="744c0-128">Indica o nome do sistema operacional e versão usada para entrar no serviço.</span><span class="sxs-lookup"><span data-stu-id="744c0-128">Indicates the OS name and version used for signing-in.</span></span>|
|<span data-ttu-id="744c0-129">trustType</span><span class="sxs-lookup"><span data-stu-id="744c0-129">trustType</span></span>|<span data-ttu-id="744c0-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="744c0-130">String</span></span>|<span data-ttu-id="744c0-131">Indica se o dispositivo conectado é integrado ao domínio local de trabalho associado, AzureAD ingressado, as informações.</span><span class="sxs-lookup"><span data-stu-id="744c0-131">Indicates information on whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="744c0-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="744c0-132">JSON representation</span></span>

<span data-ttu-id="744c0-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="744c0-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "browser": "String",
  "deviceId": "String",
  "displayName": "String",
  "isCompliant": true,
  "isManaged": true,
  "operatingSystem": "String",
  "trustType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
