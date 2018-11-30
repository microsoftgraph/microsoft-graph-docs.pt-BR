---
title: tipo de recurso microsoftStoreForBusinessAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.
ms.openlocfilehash: 62224841548c01ce84901251ab67204b82cbb4c9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007398"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="a342f-103">tipo de recurso microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="a342f-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="a342f-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a342f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a342f-105">Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.</span><span class="sxs-lookup"><span data-stu-id="a342f-105">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>

<span data-ttu-id="a342f-106">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a342f-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a342f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a342f-107">Properties</span></span>
|<span data-ttu-id="a342f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a342f-108">Property</span></span>|<span data-ttu-id="a342f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a342f-109">Type</span></span>|<span data-ttu-id="a342f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a342f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a342f-111">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="a342f-111">useDeviceContext</span></span>|<span data-ttu-id="a342f-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="a342f-112">Boolean</span></span>|<span data-ttu-id="a342f-113">Se é para usar ou não o contexto de execução do dispositivo em aplicativo móvel da Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="a342f-113">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a342f-114">Relações</span><span class="sxs-lookup"><span data-stu-id="a342f-114">Relationships</span></span>
<span data-ttu-id="a342f-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a342f-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a342f-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a342f-116">JSON Representation</span></span>
<span data-ttu-id="a342f-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a342f-117">Here is a JSON representation of the resource.</span></span>
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



