---
title: tipo de recurso deviceManagementTroubleshootingErrorResource
description: Objeto representando um link para informações de solução de problemas, o link pode ser para o portal do Azure ou um documento Microsoft.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 60a098774f8302ec23322fc18af1998ba6e14480
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43388241"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="c7753-103">tipo de recurso deviceManagementTroubleshootingErrorResource</span><span class="sxs-lookup"><span data-stu-id="c7753-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

<span data-ttu-id="c7753-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7753-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7753-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7753-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7753-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7753-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7753-107">Objeto representando um link para informações de solução de problemas, o link pode ser para o portal do Azure ou um documento Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c7753-107">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="c7753-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7753-108">Properties</span></span>
|<span data-ttu-id="c7753-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7753-109">Property</span></span>|<span data-ttu-id="c7753-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7753-110">Type</span></span>|<span data-ttu-id="c7753-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7753-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7753-112">texto</span><span class="sxs-lookup"><span data-stu-id="c7753-112">text</span></span>|<span data-ttu-id="c7753-113">String</span><span class="sxs-lookup"><span data-stu-id="c7753-113">String</span></span>|<span data-ttu-id="c7753-114">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c7753-114">Not yet documented</span></span>|
|<span data-ttu-id="c7753-115">vínculo</span><span class="sxs-lookup"><span data-stu-id="c7753-115">link</span></span>|<span data-ttu-id="c7753-116">String</span><span class="sxs-lookup"><span data-stu-id="c7753-116">String</span></span>|<span data-ttu-id="c7753-117">O link para o recurso da Web.</span><span class="sxs-lookup"><span data-stu-id="c7753-117">The link to the web resource.</span></span> <span data-ttu-id="c7753-118">Pode conter qualquer um dos seguintes formatadores: {{UPN}}, {{DeviceGUID}}, {{userguid}}</span><span class="sxs-lookup"><span data-stu-id="c7753-118">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7753-119">Relações</span><span class="sxs-lookup"><span data-stu-id="c7753-119">Relationships</span></span>
<span data-ttu-id="c7753-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c7753-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7753-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7753-121">JSON Representation</span></span>
<span data-ttu-id="c7753-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7753-122">Here is a JSON representation of the resource.</span></span>
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



