---
title: Tipo de recurso iosLobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e364ae3ef38bd01376d937c6538ce00c39ba6172
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755151"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="99162-103">Tipo de recurso iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="99162-103">iosLobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="99162-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99162-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99162-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99162-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99162-106">Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.</span><span class="sxs-lookup"><span data-stu-id="99162-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="99162-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="99162-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="99162-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99162-108">Properties</span></span>
|<span data-ttu-id="99162-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99162-109">Property</span></span>|<span data-ttu-id="99162-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="99162-110">Type</span></span>|<span data-ttu-id="99162-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="99162-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99162-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="99162-112">vpnConfigurationId</span></span>|<span data-ttu-id="99162-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99162-113">String</span></span>|<span data-ttu-id="99162-114">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="99162-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99162-115">Relações</span><span class="sxs-lookup"><span data-stu-id="99162-115">Relationships</span></span>
<span data-ttu-id="99162-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="99162-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99162-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99162-117">JSON Representation</span></span>
<span data-ttu-id="99162-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99162-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```




