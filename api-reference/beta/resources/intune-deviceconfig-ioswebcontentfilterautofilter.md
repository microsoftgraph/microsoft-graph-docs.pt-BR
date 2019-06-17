---
title: tipo de recurso iosWebContentFilterAutoFilter
description: Representa um tipo de configuração de filtro de conteúdo da Web iOS, que habilita o recurso de filtro automático do iOS e permite o controle de acesso à URL adicional. Quando construído sem valores de propriedade, o dispositivo iOS habilitará o filtro automático independentemente.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 90a94273e6675187c7aa02cc89d793f38c34516e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34985392"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="bc58d-104">tipo de recurso iosWebContentFilterAutoFilter</span><span class="sxs-lookup"><span data-stu-id="bc58d-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="bc58d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bc58d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc58d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc58d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc58d-107">Representa um tipo de configuração de filtro de conteúdo da Web iOS, que habilita o recurso de filtro automático do iOS e permite o controle de acesso à URL adicional.</span><span class="sxs-lookup"><span data-stu-id="bc58d-107">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="bc58d-108">Quando construído sem valores de propriedade, o dispositivo iOS habilitará o filtro automático independentemente.</span><span class="sxs-lookup"><span data-stu-id="bc58d-108">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>


<span data-ttu-id="bc58d-109">Herda de [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="bc58d-109">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bc58d-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc58d-110">Properties</span></span>
|<span data-ttu-id="bc58d-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc58d-111">Property</span></span>|<span data-ttu-id="bc58d-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc58d-112">Type</span></span>|<span data-ttu-id="bc58d-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc58d-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc58d-114">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="bc58d-114">allowedUrls</span></span>|<span data-ttu-id="bc58d-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc58d-115">String collection</span></span>|<span data-ttu-id="bc58d-116">URLs adicionais permitidas para acesso</span><span class="sxs-lookup"><span data-stu-id="bc58d-116">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="bc58d-117">blockedUrls</span><span class="sxs-lookup"><span data-stu-id="bc58d-117">blockedUrls</span></span>|<span data-ttu-id="bc58d-118">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc58d-118">String collection</span></span>|<span data-ttu-id="bc58d-119">URLs adicionais bloqueadas para acesso</span><span class="sxs-lookup"><span data-stu-id="bc58d-119">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc58d-120">Relações</span><span class="sxs-lookup"><span data-stu-id="bc58d-120">Relationships</span></span>
<span data-ttu-id="bc58d-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bc58d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc58d-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc58d-122">JSON Representation</span></span>
<span data-ttu-id="bc58d-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc58d-123">Here is a JSON representation of the resource.</span></span>
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





