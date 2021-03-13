---
title: Tipo de recurso deviceDetail
description: Indica os detalhes do dispositivo associados a um dispositivo usado para entrar.
localization_priority: Normal
author: spunukol
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3fb6b338793b77e3079922cd8c372e402488a22c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761125"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="408d8-103">Tipo de recurso deviceDetail</span><span class="sxs-lookup"><span data-stu-id="408d8-103">deviceDetail resource type</span></span>

<span data-ttu-id="408d8-104">Namespace: microsoft.graph Indica detalhes do dispositivo associados a um dispositivo usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="408d8-104">Namespace: microsoft.graph Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="408d8-105">Inclui informações como navegador de dispositivos e informações do sistema operacional, se o dispositivo for gerenciado pelo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="408d8-105">Includes information like device browser and  OS info, if device is Azure AD managed.</span></span>



## <a name="properties"></a><span data-ttu-id="408d8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="408d8-106">Properties</span></span>
| <span data-ttu-id="408d8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="408d8-107">Property</span></span>     | <span data-ttu-id="408d8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="408d8-108">Type</span></span>   |<span data-ttu-id="408d8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="408d8-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="408d8-110">Navegador</span><span class="sxs-lookup"><span data-stu-id="408d8-110">browser</span></span>|<span data-ttu-id="408d8-111">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="408d8-111">String</span></span>|<span data-ttu-id="408d8-112">Indica as informações do navegador do usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="408d8-112">Indicates the browser information of the used for signing-in.</span></span>|
|<span data-ttu-id="408d8-113">deviceId</span><span class="sxs-lookup"><span data-stu-id="408d8-113">deviceId</span></span>|<span data-ttu-id="408d8-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="408d8-114">String</span></span>|<span data-ttu-id="408d8-115">Refere-se à UniqueID do dispositivo usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="408d8-115">Refers to the UniqueID of the device used for signing-in.</span></span>|
|<span data-ttu-id="408d8-116">displayName</span><span class="sxs-lookup"><span data-stu-id="408d8-116">displayName</span></span>|<span data-ttu-id="408d8-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="408d8-117">String</span></span>|<span data-ttu-id="408d8-118">Refere-se ao nome do dispositivo usado para entrar.</span><span class="sxs-lookup"><span data-stu-id="408d8-118">Refers to the name of the device used for signing-in.</span></span>|
|<span data-ttu-id="408d8-119">isCompliant</span><span class="sxs-lookup"><span data-stu-id="408d8-119">isCompliant</span></span>|<span data-ttu-id="408d8-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="408d8-120">Boolean</span></span>|<span data-ttu-id="408d8-121">Indica se o dispositivo está em conformidade ou não.</span><span class="sxs-lookup"><span data-stu-id="408d8-121">Indicates whether the device is compliant or not.</span></span>|
|<span data-ttu-id="408d8-122">isManaged</span><span class="sxs-lookup"><span data-stu-id="408d8-122">isManaged</span></span>|<span data-ttu-id="408d8-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="408d8-123">Boolean</span></span>|<span data-ttu-id="408d8-124">Indica se o dispositivo é gerenciado ou não.</span><span class="sxs-lookup"><span data-stu-id="408d8-124">Indicates if the device is managed or not.</span></span>|
|<span data-ttu-id="408d8-125">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="408d8-125">operatingSystem</span></span>|<span data-ttu-id="408d8-126">String</span><span class="sxs-lookup"><span data-stu-id="408d8-126">String</span></span>|<span data-ttu-id="408d8-127">Indica o nome e a versão do sistema operacional usados para entrar.</span><span class="sxs-lookup"><span data-stu-id="408d8-127">Indicates the OS name and version used for signing-in.</span></span>|
|<span data-ttu-id="408d8-128">trustType</span><span class="sxs-lookup"><span data-stu-id="408d8-128">trustType</span></span>|<span data-ttu-id="408d8-129">String</span><span class="sxs-lookup"><span data-stu-id="408d8-129">String</span></span>|<span data-ttu-id="408d8-130">Indica informações sobre se o dispositivo conectado é Workplace Joined, AzureAD Joined, Domain Joined.</span><span class="sxs-lookup"><span data-stu-id="408d8-130">Indicates information on whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="408d8-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="408d8-131">JSON representation</span></span>

<span data-ttu-id="408d8-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="408d8-132">Here is a JSON representation of the resource.</span></span>

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


