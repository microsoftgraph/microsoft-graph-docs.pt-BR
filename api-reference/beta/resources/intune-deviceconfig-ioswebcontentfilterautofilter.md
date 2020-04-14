---
title: tipo de recurso iosWebContentFilterAutoFilter
description: Representa um tipo de configuração de filtro de conteúdo da Web iOS, que habilita o recurso de filtro automático do iOS e permite o controle de acesso à URL adicional. Quando construído sem valores de propriedade, o dispositivo iOS habilitará o filtro automático independentemente.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 01063b5709b0e10730e542f00149d6c6e3320d0a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440067"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="e0754-104">tipo de recurso iosWebContentFilterAutoFilter</span><span class="sxs-lookup"><span data-stu-id="e0754-104">iosWebContentFilterAutoFilter resource type</span></span>

<span data-ttu-id="e0754-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0754-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0754-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e0754-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0754-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e0754-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0754-108">Representa um tipo de configuração de filtro de conteúdo da Web iOS, que habilita o recurso de filtro automático do iOS e permite o controle de acesso à URL adicional.</span><span class="sxs-lookup"><span data-stu-id="e0754-108">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="e0754-109">Quando construído sem valores de propriedade, o dispositivo iOS habilitará o filtro automático independentemente.</span><span class="sxs-lookup"><span data-stu-id="e0754-109">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>


<span data-ttu-id="e0754-110">Herda de [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="e0754-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e0754-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e0754-111">Properties</span></span>
|<span data-ttu-id="e0754-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0754-112">Property</span></span>|<span data-ttu-id="e0754-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0754-113">Type</span></span>|<span data-ttu-id="e0754-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0754-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0754-115">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="e0754-115">allowedUrls</span></span>|<span data-ttu-id="e0754-116">Coleção String</span><span class="sxs-lookup"><span data-stu-id="e0754-116">String collection</span></span>|<span data-ttu-id="e0754-117">URLs adicionais permitidas para acesso</span><span class="sxs-lookup"><span data-stu-id="e0754-117">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="e0754-118">blockedUrls</span><span class="sxs-lookup"><span data-stu-id="e0754-118">blockedUrls</span></span>|<span data-ttu-id="e0754-119">Coleção String</span><span class="sxs-lookup"><span data-stu-id="e0754-119">String collection</span></span>|<span data-ttu-id="e0754-120">URLs adicionais bloqueadas para acesso</span><span class="sxs-lookup"><span data-stu-id="e0754-120">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0754-121">Relações</span><span class="sxs-lookup"><span data-stu-id="e0754-121">Relationships</span></span>
<span data-ttu-id="e0754-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e0754-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0754-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e0754-123">JSON Representation</span></span>
<span data-ttu-id="e0754-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e0754-124">Here is a JSON representation of the resource.</span></span>
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



