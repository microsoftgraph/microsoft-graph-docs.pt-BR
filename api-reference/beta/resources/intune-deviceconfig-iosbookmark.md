---
title: tipo de recurso iosBookmark
description: indicador de URL iOS
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c8a4ff93674f9fedbed0597fb8e418a59b9ea70
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946557"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="bfed2-103">tipo de recurso iosBookmark</span><span class="sxs-lookup"><span data-stu-id="bfed2-103">iosBookmark resource type</span></span>

> <span data-ttu-id="bfed2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bfed2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bfed2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bfed2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfed2-106">indicador de URL iOS</span><span class="sxs-lookup"><span data-stu-id="bfed2-106">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="bfed2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bfed2-107">Properties</span></span>
|<span data-ttu-id="bfed2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bfed2-108">Property</span></span>|<span data-ttu-id="bfed2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfed2-109">Type</span></span>|<span data-ttu-id="bfed2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfed2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfed2-111">url</span><span class="sxs-lookup"><span data-stu-id="bfed2-111">url</span></span>|<span data-ttu-id="bfed2-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bfed2-112">String</span></span>|<span data-ttu-id="bfed2-113">URL com permissão para acessar</span><span class="sxs-lookup"><span data-stu-id="bfed2-113">URL allowed to access</span></span>|
|<span data-ttu-id="bfed2-114">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="bfed2-114">bookmarkFolder</span></span>|<span data-ttu-id="bfed2-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bfed2-115">String</span></span>|<span data-ttu-id="bfed2-116">A pasta na qual o indicador deve ser adicionado no Safari</span><span class="sxs-lookup"><span data-stu-id="bfed2-116">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="bfed2-117">displayName</span><span class="sxs-lookup"><span data-stu-id="bfed2-117">displayName</span></span>|<span data-ttu-id="bfed2-118">String</span><span class="sxs-lookup"><span data-stu-id="bfed2-118">String</span></span>|<span data-ttu-id="bfed2-119">O nome de exibição do indicador</span><span class="sxs-lookup"><span data-stu-id="bfed2-119">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfed2-120">Relações</span><span class="sxs-lookup"><span data-stu-id="bfed2-120">Relationships</span></span>
<span data-ttu-id="bfed2-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bfed2-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bfed2-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bfed2-122">JSON Representation</span></span>
<span data-ttu-id="bfed2-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bfed2-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosBookmark"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosBookmark",
  "url": "String",
  "bookmarkFolder": "String",
  "displayName": "String"
}
```




