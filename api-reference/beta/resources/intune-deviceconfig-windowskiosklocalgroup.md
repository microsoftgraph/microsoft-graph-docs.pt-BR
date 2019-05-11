---
title: tipo de recurso windowsKioskLocalGroup
description: A classe usada para identificar um grupo local para a configuração do quiosque
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ab9875759c8610f976e4aaa7cc5fc8733b20ee0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943855"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="fa5cd-103">tipo de recurso windowsKioskLocalGroup</span><span class="sxs-lookup"><span data-stu-id="fa5cd-103">windowsKioskLocalGroup resource type</span></span>

> <span data-ttu-id="fa5cd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fa5cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa5cd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fa5cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa5cd-106">A classe usada para identificar um grupo local para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="fa5cd-106">The class used to identify a local group for the kiosk configuration</span></span>


<span data-ttu-id="fa5cd-107">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="fa5cd-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fa5cd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa5cd-108">Properties</span></span>
|<span data-ttu-id="fa5cd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa5cd-109">Property</span></span>|<span data-ttu-id="fa5cd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa5cd-110">Type</span></span>|<span data-ttu-id="fa5cd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa5cd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa5cd-112">Nome_do_grupo</span><span class="sxs-lookup"><span data-stu-id="fa5cd-112">groupName</span></span>|<span data-ttu-id="fa5cd-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa5cd-113">String</span></span>|<span data-ttu-id="fa5cd-114">O nome do grupo local que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="fa5cd-114">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa5cd-115">Relações</span><span class="sxs-lookup"><span data-stu-id="fa5cd-115">Relationships</span></span>
<span data-ttu-id="fa5cd-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fa5cd-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa5cd-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa5cd-117">JSON Representation</span></span>
<span data-ttu-id="fa5cd-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fa5cd-118">Here is a JSON representation of the resource.</span></span>
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




