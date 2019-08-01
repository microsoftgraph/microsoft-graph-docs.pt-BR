---
title: Tipo de recurso appListItem
description: Representa um aplicativo na lista de aplicativos gerenciados
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5b9aa0a35767078b7c91f72b7a8b06a450cc9f33
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028606"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="a0ac9-103">Tipo de recurso appListItem</span><span class="sxs-lookup"><span data-stu-id="a0ac9-103">appListItem resource type</span></span>

> <span data-ttu-id="a0ac9-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0ac9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0ac9-105">Representa um aplicativo na lista de aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="a0ac9-105">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="a0ac9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0ac9-106">Properties</span></span>
|<span data-ttu-id="a0ac9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0ac9-107">Property</span></span>|<span data-ttu-id="a0ac9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0ac9-108">Type</span></span>|<span data-ttu-id="a0ac9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0ac9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0ac9-110">name</span><span class="sxs-lookup"><span data-stu-id="a0ac9-110">name</span></span>|<span data-ttu-id="a0ac9-111">String</span><span class="sxs-lookup"><span data-stu-id="a0ac9-111">String</span></span>|<span data-ttu-id="a0ac9-112">O nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0ac9-112">The application name</span></span>|
|<span data-ttu-id="a0ac9-113">distribuidor</span><span class="sxs-lookup"><span data-stu-id="a0ac9-113">publisher</span></span>|<span data-ttu-id="a0ac9-114">String</span><span class="sxs-lookup"><span data-stu-id="a0ac9-114">String</span></span>|<span data-ttu-id="a0ac9-115">O distribuidor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0ac9-115">The publisher of the application</span></span>|
|<span data-ttu-id="a0ac9-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="a0ac9-116">appStoreUrl</span></span>|<span data-ttu-id="a0ac9-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0ac9-117">String</span></span>|<span data-ttu-id="a0ac9-118">A URL da loja do aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0ac9-118">The Store URL of the application</span></span>|
|<span data-ttu-id="a0ac9-119">appId</span><span class="sxs-lookup"><span data-stu-id="a0ac9-119">appId</span></span>|<span data-ttu-id="a0ac9-120">String</span><span class="sxs-lookup"><span data-stu-id="a0ac9-120">String</span></span>|<span data-ttu-id="a0ac9-121">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0ac9-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0ac9-122">Relações</span><span class="sxs-lookup"><span data-stu-id="a0ac9-122">Relationships</span></span>
<span data-ttu-id="a0ac9-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a0ac9-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0ac9-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0ac9-124">JSON Representation</span></span>
<span data-ttu-id="a0ac9-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0ac9-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```



