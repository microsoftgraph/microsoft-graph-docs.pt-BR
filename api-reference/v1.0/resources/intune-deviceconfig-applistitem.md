---
title: Tipo de recurso appListItem
description: Representa um aplicativo na lista de aplicativos gerenciados
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb81c8edfae3f9b33be4636e9fd7f15fa758e789
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575090"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="10084-103">Tipo de recurso appListItem</span><span class="sxs-lookup"><span data-stu-id="10084-103">appListItem resource type</span></span>

> <span data-ttu-id="10084-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="10084-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10084-105">Representa um aplicativo na lista de aplicativos gerenciados</span><span class="sxs-lookup"><span data-stu-id="10084-105">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="10084-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10084-106">Properties</span></span>
|<span data-ttu-id="10084-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10084-107">Property</span></span>|<span data-ttu-id="10084-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="10084-108">Type</span></span>|<span data-ttu-id="10084-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="10084-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10084-110">name</span><span class="sxs-lookup"><span data-stu-id="10084-110">name</span></span>|<span data-ttu-id="10084-111">String</span><span class="sxs-lookup"><span data-stu-id="10084-111">String</span></span>|<span data-ttu-id="10084-112">O nome do aplicativo</span><span class="sxs-lookup"><span data-stu-id="10084-112">The application name</span></span>|
|<span data-ttu-id="10084-113">distribuidor</span><span class="sxs-lookup"><span data-stu-id="10084-113">publisher</span></span>|<span data-ttu-id="10084-114">String</span><span class="sxs-lookup"><span data-stu-id="10084-114">String</span></span>|<span data-ttu-id="10084-115">O distribuidor do aplicativo</span><span class="sxs-lookup"><span data-stu-id="10084-115">The publisher of the application</span></span>|
|<span data-ttu-id="10084-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="10084-116">appStoreUrl</span></span>|<span data-ttu-id="10084-117">String</span><span class="sxs-lookup"><span data-stu-id="10084-117">String</span></span>|<span data-ttu-id="10084-118">A URL da loja do aplicativo</span><span class="sxs-lookup"><span data-stu-id="10084-118">The Store URL of the application</span></span>|
|<span data-ttu-id="10084-119">appId</span><span class="sxs-lookup"><span data-stu-id="10084-119">appId</span></span>|<span data-ttu-id="10084-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10084-120">String</span></span>|<span data-ttu-id="10084-121">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="10084-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="10084-122">Relações</span><span class="sxs-lookup"><span data-stu-id="10084-122">Relationships</span></span>
<span data-ttu-id="10084-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="10084-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10084-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10084-124">JSON Representation</span></span>
<span data-ttu-id="10084-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10084-125">Here is a JSON representation of the resource.</span></span>
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



