---
title: tipo de recurso deviceManagementTroubleshootingErrorResource
description: Objeto representando um link para informações de solução de problemas, o link pode ser para o portal do Azure ou um documento Microsoft.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6454bad98938bc73d4cde8d48229f6146d07c0bb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010299"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="76179-103">tipo de recurso deviceManagementTroubleshootingErrorResource</span><span class="sxs-lookup"><span data-stu-id="76179-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

> <span data-ttu-id="76179-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="76179-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76179-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76179-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76179-106">Objeto representando um link para informações de solução de problemas, o link pode ser para o portal do Azure ou um documento Microsoft.</span><span class="sxs-lookup"><span data-stu-id="76179-106">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="76179-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="76179-107">Properties</span></span>
|<span data-ttu-id="76179-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76179-108">Property</span></span>|<span data-ttu-id="76179-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="76179-109">Type</span></span>|<span data-ttu-id="76179-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="76179-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76179-111">texto</span><span class="sxs-lookup"><span data-stu-id="76179-111">text</span></span>|<span data-ttu-id="76179-112">String</span><span class="sxs-lookup"><span data-stu-id="76179-112">String</span></span>|<span data-ttu-id="76179-113">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="76179-113">Not yet documented</span></span>|
|<span data-ttu-id="76179-114">vínculo</span><span class="sxs-lookup"><span data-stu-id="76179-114">link</span></span>|<span data-ttu-id="76179-115">String</span><span class="sxs-lookup"><span data-stu-id="76179-115">String</span></span>|<span data-ttu-id="76179-116">O link para o recurso da Web.</span><span class="sxs-lookup"><span data-stu-id="76179-116">The link to the web resource.</span></span> <span data-ttu-id="76179-117">Pode conter qualquer um dos seguintes formatadores: {{UPN}}, {{DeviceGUID}}, {{userguid}}</span><span class="sxs-lookup"><span data-stu-id="76179-117">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="76179-118">Relações</span><span class="sxs-lookup"><span data-stu-id="76179-118">Relationships</span></span>
<span data-ttu-id="76179-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="76179-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76179-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="76179-120">JSON Representation</span></span>
<span data-ttu-id="76179-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="76179-121">Here is a JSON representation of the resource.</span></span>
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





