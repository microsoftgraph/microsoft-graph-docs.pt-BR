---
title: tipo de recurso iosWebContentFilterAutoFilter
description: Representa um tipo de configuração de filtro de conteúdo da Web iOS, que habilita o recurso de filtro automático do iOS e permite o controle de acesso à URL adicional. Quando construído sem valores de propriedade, o dispositivo iOS habilitará o filtro automático independentemente.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb6bf2da4320c228123e24ae67bd21b13f2c21eb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946067"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="56452-104">tipo de recurso iosWebContentFilterAutoFilter</span><span class="sxs-lookup"><span data-stu-id="56452-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="56452-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="56452-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56452-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="56452-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56452-107">Representa um tipo de configuração de filtro de conteúdo da Web iOS, que habilita o recurso de filtro automático do iOS e permite o controle de acesso à URL adicional.</span><span class="sxs-lookup"><span data-stu-id="56452-107">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="56452-108">Quando construído sem valores de propriedade, o dispositivo iOS habilitará o filtro automático independentemente.</span><span class="sxs-lookup"><span data-stu-id="56452-108">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>


<span data-ttu-id="56452-109">Herda de [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="56452-109">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="56452-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56452-110">Properties</span></span>
|<span data-ttu-id="56452-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56452-111">Property</span></span>|<span data-ttu-id="56452-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="56452-112">Type</span></span>|<span data-ttu-id="56452-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="56452-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56452-114">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="56452-114">allowedUrls</span></span>|<span data-ttu-id="56452-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="56452-115">String collection</span></span>|<span data-ttu-id="56452-116">URLs adicionais permitidas para acesso</span><span class="sxs-lookup"><span data-stu-id="56452-116">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="56452-117">blockedUrls</span><span class="sxs-lookup"><span data-stu-id="56452-117">blockedUrls</span></span>|<span data-ttu-id="56452-118">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="56452-118">String collection</span></span>|<span data-ttu-id="56452-119">URLs adicionais bloqueadas para acesso</span><span class="sxs-lookup"><span data-stu-id="56452-119">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="56452-120">Relações</span><span class="sxs-lookup"><span data-stu-id="56452-120">Relationships</span></span>
<span data-ttu-id="56452-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="56452-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56452-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56452-122">JSON Representation</span></span>
<span data-ttu-id="56452-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="56452-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterAutoFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterAutoFilter",
  "allowedUrls": [
    "String"
  ],
  "blockedUrls": [
    "String"
  ]
}
```




