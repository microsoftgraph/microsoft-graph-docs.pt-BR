---
title: tipo de recurso windowsKioskLocalGroup
description: A classe usada para identificar um grupo local para a configuração do quiosque
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7385fd0990fc7ac135a3ea9ba318e06571ecdd6d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444091"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="cfbcd-103">tipo de recurso windowsKioskLocalGroup</span><span class="sxs-lookup"><span data-stu-id="cfbcd-103">windowsKioskLocalGroup resource type</span></span>

<span data-ttu-id="cfbcd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfbcd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cfbcd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cfbcd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfbcd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cfbcd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfbcd-107">A classe usada para identificar um grupo local para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="cfbcd-107">The class used to identify a local group for the kiosk configuration</span></span>


<span data-ttu-id="cfbcd-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="cfbcd-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cfbcd-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cfbcd-109">Properties</span></span>
|<span data-ttu-id="cfbcd-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfbcd-110">Property</span></span>|<span data-ttu-id="cfbcd-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfbcd-111">Type</span></span>|<span data-ttu-id="cfbcd-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfbcd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfbcd-113">Nome_do_grupo</span><span class="sxs-lookup"><span data-stu-id="cfbcd-113">groupName</span></span>|<span data-ttu-id="cfbcd-114">String</span><span class="sxs-lookup"><span data-stu-id="cfbcd-114">String</span></span>|<span data-ttu-id="cfbcd-115">O nome do grupo local que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="cfbcd-115">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfbcd-116">Relações</span><span class="sxs-lookup"><span data-stu-id="cfbcd-116">Relationships</span></span>
<span data-ttu-id="cfbcd-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cfbcd-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfbcd-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cfbcd-118">JSON Representation</span></span>
<span data-ttu-id="cfbcd-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cfbcd-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalGroup",
  "groupName": "String"
}
```



