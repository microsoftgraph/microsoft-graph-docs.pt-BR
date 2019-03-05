---
title: tipo de recurso microsoftStoreForBusinessAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6fdcf4633433f471383e4c5b1c670eb5f5a8cb37
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164922"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="c0833-103">tipo de recurso microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="c0833-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="c0833-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c0833-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0833-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0833-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0833-106">Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.</span><span class="sxs-lookup"><span data-stu-id="c0833-106">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="c0833-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="c0833-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c0833-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c0833-108">Properties</span></span>
|<span data-ttu-id="c0833-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0833-109">Property</span></span>|<span data-ttu-id="c0833-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0833-110">Type</span></span>|<span data-ttu-id="c0833-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0833-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0833-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="c0833-112">useDeviceContext</span></span>|<span data-ttu-id="c0833-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="c0833-113">Boolean</span></span>|<span data-ttu-id="c0833-114">Se é para usar ou não o contexto de execução do dispositivo em aplicativo móvel da Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="c0833-114">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0833-115">Relações</span><span class="sxs-lookup"><span data-stu-id="c0833-115">Relationships</span></span>
<span data-ttu-id="c0833-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c0833-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0833-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c0833-117">JSON Representation</span></span>
<span data-ttu-id="c0833-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c0833-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings",
  "useDeviceContext": true
}
```




