---
title: tipo de recurso deviceDetail
description: Indica os detalhes do dispositivo associados a um dispositivo usado para entrar. Isso inclui informações como navegador de dispositivos e sistema operacional e se o dispositivo é gerenciado pelo Azure AD.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8730c6fefebadbd2c64937366c7b7de41537b11c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531668"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="14d2b-104">tipo de recurso deviceDetail</span><span class="sxs-lookup"><span data-stu-id="14d2b-104">deviceDetail resource type</span></span>

<span data-ttu-id="14d2b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14d2b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="14d2b-106">Indica os detalhes do dispositivo associados a um dispositivo usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="14d2b-106">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="14d2b-107">Isso inclui informações como navegador de dispositivos e sistema operacional e se o dispositivo é gerenciado pelo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="14d2b-107">This includes information like device browser and  operating system, and whether the device is Azure AD managed.</span></span>

## <a name="properties"></a><span data-ttu-id="14d2b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="14d2b-108">Properties</span></span>

| <span data-ttu-id="14d2b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14d2b-109">Property</span></span>     | <span data-ttu-id="14d2b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="14d2b-110">Type</span></span>   |<span data-ttu-id="14d2b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="14d2b-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14d2b-112">Navegador</span><span class="sxs-lookup"><span data-stu-id="14d2b-112">browser</span></span>|<span data-ttu-id="14d2b-113">String</span><span class="sxs-lookup"><span data-stu-id="14d2b-113">String</span></span>|<span data-ttu-id="14d2b-114">Indica as informações do navegador do usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="14d2b-114">Indicates the browser information of the used for signing in.</span></span>|
|<span data-ttu-id="14d2b-115">deviceId</span><span class="sxs-lookup"><span data-stu-id="14d2b-115">deviceId</span></span>|<span data-ttu-id="14d2b-116">String</span><span class="sxs-lookup"><span data-stu-id="14d2b-116">String</span></span>|<span data-ttu-id="14d2b-117">Refere-se ao UniqueID do dispositivo usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="14d2b-117">Refers to the UniqueID of the device used for signing in.</span></span>|
|<span data-ttu-id="14d2b-118">displayName</span><span class="sxs-lookup"><span data-stu-id="14d2b-118">displayName</span></span>|<span data-ttu-id="14d2b-119">String</span><span class="sxs-lookup"><span data-stu-id="14d2b-119">String</span></span>|<span data-ttu-id="14d2b-120">Refere-se ao nome do dispositivo usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="14d2b-120">Refers to the name of the device used for signing in.</span></span>|
|<span data-ttu-id="14d2b-121">isCompliant</span><span class="sxs-lookup"><span data-stu-id="14d2b-121">isCompliant</span></span>|<span data-ttu-id="14d2b-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="14d2b-122">Boolean</span></span>|<span data-ttu-id="14d2b-123">Indica se o dispositivo está em conformidade.</span><span class="sxs-lookup"><span data-stu-id="14d2b-123">Indicates whether the device is compliant.</span></span>|
|<span data-ttu-id="14d2b-124">isManaged</span><span class="sxs-lookup"><span data-stu-id="14d2b-124">isManaged</span></span>|<span data-ttu-id="14d2b-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="14d2b-125">Boolean</span></span>|<span data-ttu-id="14d2b-126">Indica se o dispositivo é gerenciado.</span><span class="sxs-lookup"><span data-stu-id="14d2b-126">Indicates whether the device is managed.</span></span>|
|<span data-ttu-id="14d2b-127">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="14d2b-127">operatingSystem</span></span>|<span data-ttu-id="14d2b-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14d2b-128">String</span></span>|<span data-ttu-id="14d2b-129">Indica o nome do sistema operacional e a versão usada para entrar.</span><span class="sxs-lookup"><span data-stu-id="14d2b-129">Indicates the operating system name and version used for signing in.</span></span>|
|<span data-ttu-id="14d2b-130">trustType</span><span class="sxs-lookup"><span data-stu-id="14d2b-130">trustType</span></span>|<span data-ttu-id="14d2b-131">String</span><span class="sxs-lookup"><span data-stu-id="14d2b-131">String</span></span>|<span data-ttu-id="14d2b-132">Fornece informações sobre se o dispositivo conectado é um local de trabalho associado, AzureAD Unido, ingresso no domínio.</span><span class="sxs-lookup"><span data-stu-id="14d2b-132">Provides information about whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="14d2b-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="14d2b-133">JSON representation</span></span>

<span data-ttu-id="14d2b-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="14d2b-134">Here is a JSON representation of the resource.</span></span>

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
