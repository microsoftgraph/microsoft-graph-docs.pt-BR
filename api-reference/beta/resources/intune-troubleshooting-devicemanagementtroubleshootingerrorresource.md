---
title: tipo de recurso deviceManagementTroubleshootingErrorResource
description: Objeto representando um link para informações de solução de problemas, o link pode ser para o portal do Azure ou um documento Microsoft.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0dd4db93e49b274b9992bd91612c6a384daecdef
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255298"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="fe5de-103">tipo de recurso deviceManagementTroubleshootingErrorResource</span><span class="sxs-lookup"><span data-stu-id="fe5de-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

<span data-ttu-id="fe5de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe5de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe5de-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fe5de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe5de-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fe5de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe5de-107">Objeto representando um link para informações de solução de problemas, o link pode ser para o portal do Azure ou um documento Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fe5de-107">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="fe5de-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe5de-108">Properties</span></span>
|<span data-ttu-id="fe5de-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe5de-109">Property</span></span>|<span data-ttu-id="fe5de-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe5de-110">Type</span></span>|<span data-ttu-id="fe5de-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe5de-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe5de-112">texto</span><span class="sxs-lookup"><span data-stu-id="fe5de-112">text</span></span>|<span data-ttu-id="fe5de-113">String</span><span class="sxs-lookup"><span data-stu-id="fe5de-113">String</span></span>|<span data-ttu-id="fe5de-114">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fe5de-114">Not yet documented</span></span>|
|<span data-ttu-id="fe5de-115">vínculo</span><span class="sxs-lookup"><span data-stu-id="fe5de-115">link</span></span>|<span data-ttu-id="fe5de-116">String</span><span class="sxs-lookup"><span data-stu-id="fe5de-116">String</span></span>|<span data-ttu-id="fe5de-117">O link para o recurso da Web.</span><span class="sxs-lookup"><span data-stu-id="fe5de-117">The link to the web resource.</span></span> <span data-ttu-id="fe5de-118">Pode conter qualquer um dos seguintes formatadores: {{UPN}}, {{DeviceGUID}}, {{userguid}}</span><span class="sxs-lookup"><span data-stu-id="fe5de-118">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe5de-119">Relações</span><span class="sxs-lookup"><span data-stu-id="fe5de-119">Relationships</span></span>
<span data-ttu-id="fe5de-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fe5de-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe5de-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe5de-121">JSON Representation</span></span>
<span data-ttu-id="fe5de-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe5de-122">Here is a JSON representation of the resource.</span></span>
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




