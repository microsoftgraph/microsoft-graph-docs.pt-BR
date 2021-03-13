---
title: Tipo de recurso deviceDetail
description: Indica os detalhes do dispositivo associados a um dispositivo usado para entrar. Isso inclui informações como navegador de dispositivo e sistema operacional e se o dispositivo é gerenciado pelo Azure AD.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 1c48724a12f7cb29de74a965c1cbb06a44498d26
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761209"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="0b449-104">Tipo de recurso deviceDetail</span><span class="sxs-lookup"><span data-stu-id="0b449-104">deviceDetail resource type</span></span>

<span data-ttu-id="0b449-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b449-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b449-106">Indica os detalhes do dispositivo associados a um dispositivo usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="0b449-106">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="0b449-107">Isso inclui informações como navegador de dispositivo e sistema operacional e se o dispositivo é gerenciado pelo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0b449-107">This includes information like device browser and  operating system, and whether the device is Azure AD managed.</span></span>

## <a name="properties"></a><span data-ttu-id="0b449-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b449-108">Properties</span></span>

| <span data-ttu-id="0b449-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b449-109">Property</span></span>     | <span data-ttu-id="0b449-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b449-110">Type</span></span>   |<span data-ttu-id="0b449-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b449-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b449-112">Navegador</span><span class="sxs-lookup"><span data-stu-id="0b449-112">browser</span></span>|<span data-ttu-id="0b449-113">String</span><span class="sxs-lookup"><span data-stu-id="0b449-113">String</span></span>|<span data-ttu-id="0b449-114">Indica as informações do navegador do usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="0b449-114">Indicates the browser information of the used for signing in.</span></span>|
|<span data-ttu-id="0b449-115">deviceId</span><span class="sxs-lookup"><span data-stu-id="0b449-115">deviceId</span></span>|<span data-ttu-id="0b449-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b449-116">String</span></span>|<span data-ttu-id="0b449-117">Refere-se ao UniqueID do dispositivo usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="0b449-117">Refers to the UniqueID of the device used for signing in.</span></span>|
|<span data-ttu-id="0b449-118">displayName</span><span class="sxs-lookup"><span data-stu-id="0b449-118">displayName</span></span>|<span data-ttu-id="0b449-119">String</span><span class="sxs-lookup"><span data-stu-id="0b449-119">String</span></span>|<span data-ttu-id="0b449-120">Refere-se ao nome do dispositivo usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="0b449-120">Refers to the name of the device used for signing in.</span></span>|
|<span data-ttu-id="0b449-121">isCompliant</span><span class="sxs-lookup"><span data-stu-id="0b449-121">isCompliant</span></span>|<span data-ttu-id="0b449-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b449-122">Boolean</span></span>|<span data-ttu-id="0b449-123">Indica se o dispositivo é compatível.</span><span class="sxs-lookup"><span data-stu-id="0b449-123">Indicates whether the device is compliant.</span></span>|
|<span data-ttu-id="0b449-124">isManaged</span><span class="sxs-lookup"><span data-stu-id="0b449-124">isManaged</span></span>|<span data-ttu-id="0b449-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b449-125">Boolean</span></span>|<span data-ttu-id="0b449-126">Indica se o dispositivo é gerenciado.</span><span class="sxs-lookup"><span data-stu-id="0b449-126">Indicates whether the device is managed.</span></span>|
|<span data-ttu-id="0b449-127">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="0b449-127">operatingSystem</span></span>|<span data-ttu-id="0b449-128">String</span><span class="sxs-lookup"><span data-stu-id="0b449-128">String</span></span>|<span data-ttu-id="0b449-129">Indica o nome e a versão do sistema operacional usados para entrar.</span><span class="sxs-lookup"><span data-stu-id="0b449-129">Indicates the operating system name and version used for signing in.</span></span>|
|<span data-ttu-id="0b449-130">trustType</span><span class="sxs-lookup"><span data-stu-id="0b449-130">trustType</span></span>|<span data-ttu-id="0b449-131">String</span><span class="sxs-lookup"><span data-stu-id="0b449-131">String</span></span>|<span data-ttu-id="0b449-132">Fornece informações sobre se o dispositivo conectado é Workplace Joined, AzureAD Joined, Domain Joined.</span><span class="sxs-lookup"><span data-stu-id="0b449-132">Provides information about whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0b449-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b449-133">JSON representation</span></span>

<span data-ttu-id="0b449-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b449-134">Here is a JSON representation of the resource.</span></span>

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

