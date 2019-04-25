---
title: tipo de recurso deviceDetail
description: Indica os detalhes do dispositivo associados a um dispositivo usado para entrar. Inclui informações como navegador de dispositivo e informações de so, se o dispositivo for gerenciado pelo Azure AD.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 18d55e397cf6c892cd37aea930d446c630017a92
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543167"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="0d2af-104">tipo de recurso deviceDetail</span><span class="sxs-lookup"><span data-stu-id="0d2af-104">deviceDetail resource type</span></span>
<span data-ttu-id="0d2af-105">Indica os detalhes do dispositivo associados a um dispositivo usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="0d2af-105">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="0d2af-106">Inclui informações como navegador de dispositivo e informações de so, se o dispositivo for gerenciado pelo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0d2af-106">Includes information like device browser and  OS info, if device is Azure AD managed.</span></span>



## <a name="properties"></a><span data-ttu-id="0d2af-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0d2af-107">Properties</span></span>
| <span data-ttu-id="0d2af-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d2af-108">Property</span></span>     | <span data-ttu-id="0d2af-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d2af-109">Type</span></span>   |<span data-ttu-id="0d2af-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d2af-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d2af-111">Navegador</span><span class="sxs-lookup"><span data-stu-id="0d2af-111">browser</span></span>|<span data-ttu-id="0d2af-112">String</span><span class="sxs-lookup"><span data-stu-id="0d2af-112">String</span></span>|<span data-ttu-id="0d2af-113">Indica as informações do navegador do usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="0d2af-113">Indicates the browser information of the used for signing-in.</span></span>|
|<span data-ttu-id="0d2af-114">deviceId</span><span class="sxs-lookup"><span data-stu-id="0d2af-114">deviceId</span></span>|<span data-ttu-id="0d2af-115">String</span><span class="sxs-lookup"><span data-stu-id="0d2af-115">String</span></span>|<span data-ttu-id="0d2af-116">Refere-se ao UniqueID do dispositivo usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="0d2af-116">Refers to the UniqueID of the device used for signing-in.</span></span>|
|<span data-ttu-id="0d2af-117">displayName</span><span class="sxs-lookup"><span data-stu-id="0d2af-117">displayName</span></span>|<span data-ttu-id="0d2af-118">String</span><span class="sxs-lookup"><span data-stu-id="0d2af-118">String</span></span>|<span data-ttu-id="0d2af-119">Refere-se ao nome do dispositivo usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="0d2af-119">Refers to the name of the device used for signing-in.</span></span>|
|<span data-ttu-id="0d2af-120">isCompliant</span><span class="sxs-lookup"><span data-stu-id="0d2af-120">isCompliant</span></span>|<span data-ttu-id="0d2af-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="0d2af-121">Boolean</span></span>|<span data-ttu-id="0d2af-122">Indica se o dispositivo está em conformidade ou não.</span><span class="sxs-lookup"><span data-stu-id="0d2af-122">Indicates whether the device is compliant or not.</span></span>|
|<span data-ttu-id="0d2af-123">isManaged</span><span class="sxs-lookup"><span data-stu-id="0d2af-123">isManaged</span></span>|<span data-ttu-id="0d2af-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="0d2af-124">Boolean</span></span>|<span data-ttu-id="0d2af-125">Indica se o dispositivo é gerenciado ou não.</span><span class="sxs-lookup"><span data-stu-id="0d2af-125">Indicates if the device is managed or not.</span></span>|
|<span data-ttu-id="0d2af-126">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="0d2af-126">operatingSystem</span></span>|<span data-ttu-id="0d2af-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d2af-127">String</span></span>|<span data-ttu-id="0d2af-128">Indica o nome do sistema operacional e a versão usada para entrar.</span><span class="sxs-lookup"><span data-stu-id="0d2af-128">Indicates the OS name and version used for signing-in.</span></span>|
|<span data-ttu-id="0d2af-129">trustType</span><span class="sxs-lookup"><span data-stu-id="0d2af-129">trustType</span></span>|<span data-ttu-id="0d2af-130">String</span><span class="sxs-lookup"><span data-stu-id="0d2af-130">String</span></span>|<span data-ttu-id="0d2af-131">Indica informações sobre se o dispositivo conectado é membro do local de trabalho, AzureAD Unido, ingresso no domínio.</span><span class="sxs-lookup"><span data-stu-id="0d2af-131">Indicates information on whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0d2af-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0d2af-132">JSON representation</span></span>

<span data-ttu-id="0d2af-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0d2af-133">Here is a JSON representation of the resource.</span></span>

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
