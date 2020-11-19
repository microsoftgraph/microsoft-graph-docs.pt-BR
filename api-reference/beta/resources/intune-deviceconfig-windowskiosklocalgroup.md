---
title: tipo de recurso windowsKioskLocalGroup
description: A classe usada para identificar um grupo local para a configuração do quiosque
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 50ebc28381d1453fe7f178f9ede846a60f2dcf0f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49226647"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="67c37-103">tipo de recurso windowsKioskLocalGroup</span><span class="sxs-lookup"><span data-stu-id="67c37-103">windowsKioskLocalGroup resource type</span></span>

<span data-ttu-id="67c37-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67c37-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67c37-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67c37-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67c37-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67c37-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67c37-107">A classe usada para identificar um grupo local para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="67c37-107">The class used to identify a local group for the kiosk configuration</span></span>


<span data-ttu-id="67c37-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="67c37-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="67c37-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="67c37-109">Properties</span></span>
|<span data-ttu-id="67c37-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67c37-110">Property</span></span>|<span data-ttu-id="67c37-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="67c37-111">Type</span></span>|<span data-ttu-id="67c37-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="67c37-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67c37-113">Nome_do_grupo</span><span class="sxs-lookup"><span data-stu-id="67c37-113">groupName</span></span>|<span data-ttu-id="67c37-114">String</span><span class="sxs-lookup"><span data-stu-id="67c37-114">String</span></span>|<span data-ttu-id="67c37-115">O nome do grupo local que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="67c37-115">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="67c37-116">Relações</span><span class="sxs-lookup"><span data-stu-id="67c37-116">Relationships</span></span>
<span data-ttu-id="67c37-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="67c37-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67c37-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="67c37-118">JSON Representation</span></span>
<span data-ttu-id="67c37-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="67c37-119">Here is a JSON representation of the resource.</span></span>
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




