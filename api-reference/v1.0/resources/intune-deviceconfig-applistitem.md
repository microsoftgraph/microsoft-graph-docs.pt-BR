---
title: Tipo de recurso appListItem
description: Representa um aplicativo na lista de aplicativos gerenciados
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c43b559f1c1994d34ae0d4202b4970227d029df7
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366738"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="08c11-103">Tipo de recurso appListItem</span><span class="sxs-lookup"><span data-stu-id="08c11-103">appListItem resource type</span></span>

> <span data-ttu-id="08c11-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="08c11-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08c11-105">Representa um aplicativo na lista de aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="08c11-105">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="08c11-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08c11-106">Properties</span></span>
|<span data-ttu-id="08c11-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08c11-107">Property</span></span>|<span data-ttu-id="08c11-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="08c11-108">Type</span></span>|<span data-ttu-id="08c11-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="08c11-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08c11-110">name</span><span class="sxs-lookup"><span data-stu-id="08c11-110">name</span></span>|<span data-ttu-id="08c11-111">String</span><span class="sxs-lookup"><span data-stu-id="08c11-111">String</span></span>|<span data-ttu-id="08c11-112">O nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="08c11-112">The application name</span></span>|
|<span data-ttu-id="08c11-113">distribuidor</span><span class="sxs-lookup"><span data-stu-id="08c11-113">publisher</span></span>|<span data-ttu-id="08c11-114">String</span><span class="sxs-lookup"><span data-stu-id="08c11-114">String</span></span>|<span data-ttu-id="08c11-115">O distribuidor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="08c11-115">The publisher of the application</span></span>|
|<span data-ttu-id="08c11-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="08c11-116">appStoreUrl</span></span>|<span data-ttu-id="08c11-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08c11-117">String</span></span>|<span data-ttu-id="08c11-118">A URL da loja do aplicativo</span><span class="sxs-lookup"><span data-stu-id="08c11-118">The Store URL of the application</span></span>|
|<span data-ttu-id="08c11-119">appId</span><span class="sxs-lookup"><span data-stu-id="08c11-119">appId</span></span>|<span data-ttu-id="08c11-120">String</span><span class="sxs-lookup"><span data-stu-id="08c11-120">String</span></span>|<span data-ttu-id="08c11-121">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="08c11-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="08c11-122">Relações</span><span class="sxs-lookup"><span data-stu-id="08c11-122">Relationships</span></span>
<span data-ttu-id="08c11-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="08c11-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08c11-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08c11-124">JSON Representation</span></span>
<span data-ttu-id="08c11-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="08c11-125">Here is a JSON representation of the resource.</span></span>
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




