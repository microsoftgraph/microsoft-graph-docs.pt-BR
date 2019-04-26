---
title: tipo de recurso microsoftStoreForBusinessAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 64aca2bde63a3a0e4295be6eb38f1d3362e52337
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552877"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="553c3-103">tipo de recurso microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="553c3-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="553c3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="553c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="553c3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="553c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="553c3-106">Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.</span><span class="sxs-lookup"><span data-stu-id="553c3-106">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="553c3-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="553c3-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="553c3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="553c3-108">Properties</span></span>
|<span data-ttu-id="553c3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="553c3-109">Property</span></span>|<span data-ttu-id="553c3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="553c3-110">Type</span></span>|<span data-ttu-id="553c3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="553c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="553c3-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="553c3-112">useDeviceContext</span></span>|<span data-ttu-id="553c3-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="553c3-113">Boolean</span></span>|<span data-ttu-id="553c3-114">Se é para usar ou não o contexto de execução do dispositivo em aplicativo móvel da Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="553c3-114">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="553c3-115">Relações</span><span class="sxs-lookup"><span data-stu-id="553c3-115">Relationships</span></span>
<span data-ttu-id="553c3-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="553c3-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="553c3-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="553c3-117">JSON Representation</span></span>
<span data-ttu-id="553c3-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="553c3-118">Here is a JSON representation of the resource.</span></span>
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





