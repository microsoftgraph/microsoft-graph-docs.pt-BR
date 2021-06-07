---
title: Tipo de recurso iosVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 342f773d48b4918693b6062aba161ce72c82d743
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756061"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="1022c-103">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="1022c-103">iosVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="1022c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1022c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1022c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1022c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1022c-106">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="1022c-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="1022c-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="1022c-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1022c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1022c-108">Properties</span></span>
|<span data-ttu-id="1022c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1022c-109">Property</span></span>|<span data-ttu-id="1022c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1022c-110">Type</span></span>|<span data-ttu-id="1022c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1022c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1022c-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="1022c-112">useDeviceLicensing</span></span>|<span data-ttu-id="1022c-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="1022c-113">Boolean</span></span>|<span data-ttu-id="1022c-114">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1022c-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="1022c-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="1022c-115">vpnConfigurationId</span></span>|<span data-ttu-id="1022c-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1022c-116">String</span></span>|<span data-ttu-id="1022c-117">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1022c-117">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1022c-118">Relações</span><span class="sxs-lookup"><span data-stu-id="1022c-118">Relationships</span></span>
<span data-ttu-id="1022c-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="1022c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1022c-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1022c-120">JSON Representation</span></span>
<span data-ttu-id="1022c-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1022c-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String"
}
```




