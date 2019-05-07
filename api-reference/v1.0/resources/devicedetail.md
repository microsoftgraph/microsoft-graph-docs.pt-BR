---
title: tipo de recurso deviceDetail
description: Indica os detalhes do dispositivo associados a um dispositivo usado para entrar. Isso inclui informações como navegador de dispositivos e sistema operacional e se o dispositivo é gerenciado pelo Azure AD.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a6ea50eeea3a906346b69466d2686a2de101792a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629296"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="eabd8-104">tipo de recurso deviceDetail</span><span class="sxs-lookup"><span data-stu-id="eabd8-104">deviceDetail resource type</span></span>

<span data-ttu-id="eabd8-105">Indica os detalhes do dispositivo associados a um dispositivo usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="eabd8-105">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="eabd8-106">Isso inclui informações como navegador de dispositivos e sistema operacional e se o dispositivo é gerenciado pelo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eabd8-106">This includes information like device browser and  operating system, and whether the device is Azure AD managed.</span></span>

## <a name="properties"></a><span data-ttu-id="eabd8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eabd8-107">Properties</span></span>

| <span data-ttu-id="eabd8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eabd8-108">Property</span></span>     | <span data-ttu-id="eabd8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="eabd8-109">Type</span></span>   |<span data-ttu-id="eabd8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="eabd8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eabd8-111">Navegador</span><span class="sxs-lookup"><span data-stu-id="eabd8-111">browser</span></span>|<span data-ttu-id="eabd8-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eabd8-112">String</span></span>|<span data-ttu-id="eabd8-113">Indica as informações do navegador do usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="eabd8-113">Indicates the browser information of the used for signing in.</span></span>|
|<span data-ttu-id="eabd8-114">deviceId</span><span class="sxs-lookup"><span data-stu-id="eabd8-114">deviceId</span></span>|<span data-ttu-id="eabd8-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eabd8-115">String</span></span>|<span data-ttu-id="eabd8-116">Refere-se ao UniqueID do dispositivo usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="eabd8-116">Refers to the UniqueID of the device used for signing in.</span></span>|
|<span data-ttu-id="eabd8-117">displayName</span><span class="sxs-lookup"><span data-stu-id="eabd8-117">displayName</span></span>|<span data-ttu-id="eabd8-118">String</span><span class="sxs-lookup"><span data-stu-id="eabd8-118">String</span></span>|<span data-ttu-id="eabd8-119">Refere-se ao nome do dispositivo usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="eabd8-119">Refers to the name of the device used for signing in.</span></span>|
|<span data-ttu-id="eabd8-120">isCompliant</span><span class="sxs-lookup"><span data-stu-id="eabd8-120">isCompliant</span></span>|<span data-ttu-id="eabd8-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="eabd8-121">Boolean</span></span>|<span data-ttu-id="eabd8-122">Indica se o dispositivo está em conformidade.</span><span class="sxs-lookup"><span data-stu-id="eabd8-122">Indicates whether the device is compliant.</span></span>|
|<span data-ttu-id="eabd8-123">isManaged</span><span class="sxs-lookup"><span data-stu-id="eabd8-123">isManaged</span></span>|<span data-ttu-id="eabd8-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="eabd8-124">Boolean</span></span>|<span data-ttu-id="eabd8-125">Indica se o dispositivo é gerenciado.</span><span class="sxs-lookup"><span data-stu-id="eabd8-125">Indicates whether the device is managed.</span></span>|
|<span data-ttu-id="eabd8-126">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="eabd8-126">operatingSystem</span></span>|<span data-ttu-id="eabd8-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eabd8-127">String</span></span>|<span data-ttu-id="eabd8-128">Indica o nome do sistema operacional e a versão usada para entrar.</span><span class="sxs-lookup"><span data-stu-id="eabd8-128">Indicates the operating system name and version used for signing in.</span></span>|
|<span data-ttu-id="eabd8-129">trustType</span><span class="sxs-lookup"><span data-stu-id="eabd8-129">trustType</span></span>|<span data-ttu-id="eabd8-130">String</span><span class="sxs-lookup"><span data-stu-id="eabd8-130">String</span></span>|<span data-ttu-id="eabd8-131">Fornece informações sobre se o dispositivo conectado é um local de trabalho associado, AzureAD Unido, ingresso no domínio.</span><span class="sxs-lookup"><span data-stu-id="eabd8-131">Provides information about whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eabd8-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eabd8-132">JSON representation</span></span>

<span data-ttu-id="eabd8-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eabd8-133">Here is a JSON representation of the resource.</span></span>

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
