---
title: tipo de recurso deviceManagementTroubleshootingErrorResource
description: Objeto representando um link para informações de solução de problemas, o link pode ser para o portal do Azure ou um documento Microsoft.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eaf3cc39efb52bb7f603c636a69d13e3d025ce5f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347735"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="e507c-103">tipo de recurso deviceManagementTroubleshootingErrorResource</span><span class="sxs-lookup"><span data-stu-id="e507c-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

> <span data-ttu-id="e507c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e507c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e507c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e507c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e507c-106">Objeto representando um link para informações de solução de problemas, o link pode ser para o portal do Azure ou um documento Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e507c-106">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="e507c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e507c-107">Properties</span></span>
|<span data-ttu-id="e507c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e507c-108">Property</span></span>|<span data-ttu-id="e507c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e507c-109">Type</span></span>|<span data-ttu-id="e507c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e507c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e507c-111">texto</span><span class="sxs-lookup"><span data-stu-id="e507c-111">text</span></span>|<span data-ttu-id="e507c-112">String</span><span class="sxs-lookup"><span data-stu-id="e507c-112">String</span></span>|<span data-ttu-id="e507c-113">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e507c-113">Not yet documented</span></span>|
|<span data-ttu-id="e507c-114">vínculo</span><span class="sxs-lookup"><span data-stu-id="e507c-114">link</span></span>|<span data-ttu-id="e507c-115">String</span><span class="sxs-lookup"><span data-stu-id="e507c-115">String</span></span>|<span data-ttu-id="e507c-116">O link para o recurso da Web.</span><span class="sxs-lookup"><span data-stu-id="e507c-116">The link to the web resource.</span></span> <span data-ttu-id="e507c-117">Pode conter qualquer um dos seguintes formatadores: {{UPN}}, {{DeviceGUID}}, {{userguid}}</span><span class="sxs-lookup"><span data-stu-id="e507c-117">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="e507c-118">Relações</span><span class="sxs-lookup"><span data-stu-id="e507c-118">Relationships</span></span>
<span data-ttu-id="e507c-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e507c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e507c-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e507c-120">JSON Representation</span></span>
<span data-ttu-id="e507c-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e507c-121">Here is a JSON representation of the resource.</span></span>
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



