---
title: Tipo de recurso iosStoreAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 111f7a1f1a5b48e46e00ee98f95eaa7397bf6ab4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075032"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="63e6c-103">Tipo de recurso iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="63e6c-103">iosStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="63e6c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63e6c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63e6c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63e6c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63e6c-106">Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.</span><span class="sxs-lookup"><span data-stu-id="63e6c-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="63e6c-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="63e6c-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="63e6c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="63e6c-108">Properties</span></span>
|<span data-ttu-id="63e6c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63e6c-109">Property</span></span>|<span data-ttu-id="63e6c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="63e6c-110">Type</span></span>|<span data-ttu-id="63e6c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="63e6c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63e6c-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="63e6c-112">vpnConfigurationId</span></span>|<span data-ttu-id="63e6c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63e6c-113">String</span></span>|<span data-ttu-id="63e6c-114">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="63e6c-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63e6c-115">Relações</span><span class="sxs-lookup"><span data-stu-id="63e6c-115">Relationships</span></span>
<span data-ttu-id="63e6c-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="63e6c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63e6c-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="63e6c-117">JSON Representation</span></span>
<span data-ttu-id="63e6c-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="63e6c-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```









