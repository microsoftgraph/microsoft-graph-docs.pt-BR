---
title: tipo de recurso deviceDetail
description: Indica os detalhes do dispositivo associados a um dispositivo usado para entrar.
localization_priority: Normal
author: spunukol
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 69d8d1e2314021752a5f1a0ab3650d8176ecc8dc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049846"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="ac6c5-103">tipo de recurso deviceDetail</span><span class="sxs-lookup"><span data-stu-id="ac6c5-103">deviceDetail resource type</span></span>

<span data-ttu-id="ac6c5-104">Namespace: o Microsoft. Graph indica os detalhes do dispositivo associados a um dispositivo usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="ac6c5-104">Namespace: microsoft.graph Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="ac6c5-105">Inclui informações como navegador de dispositivo e informações de so, se o dispositivo for gerenciado pelo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ac6c5-105">Includes information like device browser and  OS info, if device is Azure AD managed.</span></span>



## <a name="properties"></a><span data-ttu-id="ac6c5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac6c5-106">Properties</span></span>
| <span data-ttu-id="ac6c5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac6c5-107">Property</span></span>     | <span data-ttu-id="ac6c5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac6c5-108">Type</span></span>   |<span data-ttu-id="ac6c5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac6c5-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac6c5-110">Navegador</span><span class="sxs-lookup"><span data-stu-id="ac6c5-110">browser</span></span>|<span data-ttu-id="ac6c5-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac6c5-111">String</span></span>|<span data-ttu-id="ac6c5-112">Indica as informações do navegador do usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="ac6c5-112">Indicates the browser information of the used for signing-in.</span></span>|
|<span data-ttu-id="ac6c5-113">deviceId</span><span class="sxs-lookup"><span data-stu-id="ac6c5-113">deviceId</span></span>|<span data-ttu-id="ac6c5-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac6c5-114">String</span></span>|<span data-ttu-id="ac6c5-115">Refere-se ao UniqueID do dispositivo usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="ac6c5-115">Refers to the UniqueID of the device used for signing-in.</span></span>|
|<span data-ttu-id="ac6c5-116">displayName</span><span class="sxs-lookup"><span data-stu-id="ac6c5-116">displayName</span></span>|<span data-ttu-id="ac6c5-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac6c5-117">String</span></span>|<span data-ttu-id="ac6c5-118">Refere-se ao nome do dispositivo usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="ac6c5-118">Refers to the name of the device used for signing-in.</span></span>|
|<span data-ttu-id="ac6c5-119">isCompliant</span><span class="sxs-lookup"><span data-stu-id="ac6c5-119">isCompliant</span></span>|<span data-ttu-id="ac6c5-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac6c5-120">Boolean</span></span>|<span data-ttu-id="ac6c5-121">Indica se o dispositivo está em conformidade ou não.</span><span class="sxs-lookup"><span data-stu-id="ac6c5-121">Indicates whether the device is compliant or not.</span></span>|
|<span data-ttu-id="ac6c5-122">isManaged</span><span class="sxs-lookup"><span data-stu-id="ac6c5-122">isManaged</span></span>|<span data-ttu-id="ac6c5-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac6c5-123">Boolean</span></span>|<span data-ttu-id="ac6c5-124">Indica se o dispositivo é gerenciado ou não.</span><span class="sxs-lookup"><span data-stu-id="ac6c5-124">Indicates if the device is managed or not.</span></span>|
|<span data-ttu-id="ac6c5-125">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="ac6c5-125">operatingSystem</span></span>|<span data-ttu-id="ac6c5-126">String</span><span class="sxs-lookup"><span data-stu-id="ac6c5-126">String</span></span>|<span data-ttu-id="ac6c5-127">Indica o nome do sistema operacional e a versão usada para entrar.</span><span class="sxs-lookup"><span data-stu-id="ac6c5-127">Indicates the OS name and version used for signing-in.</span></span>|
|<span data-ttu-id="ac6c5-128">trustType</span><span class="sxs-lookup"><span data-stu-id="ac6c5-128">trustType</span></span>|<span data-ttu-id="ac6c5-129">String</span><span class="sxs-lookup"><span data-stu-id="ac6c5-129">String</span></span>|<span data-ttu-id="ac6c5-130">Indica informações sobre se o dispositivo conectado é membro do local de trabalho, AzureAD Unido, ingresso no domínio.</span><span class="sxs-lookup"><span data-stu-id="ac6c5-130">Indicates information on whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ac6c5-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac6c5-131">JSON representation</span></span>

<span data-ttu-id="ac6c5-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ac6c5-132">Here is a JSON representation of the resource.</span></span>

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


