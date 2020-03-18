---
title: tipo de recurso deviceManagementTroubleshootingErrorResource
description: Objeto representando um link para informações de solução de problemas, o link pode ser para o portal do Azure ou um documento Microsoft.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5c0507a793585818e709ccbbb02cb93743e7502d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42765668"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="a49e6-103">tipo de recurso deviceManagementTroubleshootingErrorResource</span><span class="sxs-lookup"><span data-stu-id="a49e6-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

> <span data-ttu-id="a49e6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a49e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a49e6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a49e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a49e6-106">Objeto representando um link para informações de solução de problemas, o link pode ser para o portal do Azure ou um documento Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a49e6-106">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="a49e6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a49e6-107">Properties</span></span>
|<span data-ttu-id="a49e6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a49e6-108">Property</span></span>|<span data-ttu-id="a49e6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a49e6-109">Type</span></span>|<span data-ttu-id="a49e6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a49e6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a49e6-111">texto</span><span class="sxs-lookup"><span data-stu-id="a49e6-111">text</span></span>|<span data-ttu-id="a49e6-112">String</span><span class="sxs-lookup"><span data-stu-id="a49e6-112">String</span></span>|<span data-ttu-id="a49e6-113">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a49e6-113">Not yet documented</span></span>|
|<span data-ttu-id="a49e6-114">vínculo</span><span class="sxs-lookup"><span data-stu-id="a49e6-114">link</span></span>|<span data-ttu-id="a49e6-115">String</span><span class="sxs-lookup"><span data-stu-id="a49e6-115">String</span></span>|<span data-ttu-id="a49e6-116">O link para o recurso da Web.</span><span class="sxs-lookup"><span data-stu-id="a49e6-116">The link to the web resource.</span></span> <span data-ttu-id="a49e6-117">Pode conter qualquer um dos seguintes formatadores: {{UPN}}, {{DeviceGUID}}, {{userguid}}</span><span class="sxs-lookup"><span data-stu-id="a49e6-117">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="a49e6-118">Relações</span><span class="sxs-lookup"><span data-stu-id="a49e6-118">Relationships</span></span>
<span data-ttu-id="a49e6-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a49e6-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a49e6-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a49e6-120">JSON Representation</span></span>
<span data-ttu-id="a49e6-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a49e6-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorResource",
  "text": "String",
  "link": "String"
}
```



