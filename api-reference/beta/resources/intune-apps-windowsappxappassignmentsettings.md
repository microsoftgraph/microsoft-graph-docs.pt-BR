---
title: tipo de recurso de windowsAppXAppAssignmentSettings
description: Contém propriedades usadas durante a atribuição de um aplicativo móvel do Windows AppX a um grupo.
author: tfitzmac
ms.openlocfilehash: 84103a91c3c670ef3da8a0ea2a2e38a95cff79a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311617"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="d2454-103">tipo de recurso de windowsAppXAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="d2454-103">windowsAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="d2454-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d2454-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2454-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d2454-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2454-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d2454-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2454-107">Contém propriedades usadas durante a atribuição de um aplicativo móvel do Windows AppX a um grupo.</span><span class="sxs-lookup"><span data-stu-id="d2454-107">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>

<span data-ttu-id="d2454-108">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="d2454-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d2454-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2454-109">Properties</span></span>
|<span data-ttu-id="d2454-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2454-110">Property</span></span>|<span data-ttu-id="d2454-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2454-111">Type</span></span>|<span data-ttu-id="d2454-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2454-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2454-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="d2454-113">useDeviceContext</span></span>|<span data-ttu-id="d2454-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="d2454-114">Boolean</span></span>|<span data-ttu-id="d2454-115">Se deseja ou não usar o contexto de execução do dispositivo para o aplicativo móvel do Windows AppX.</span><span class="sxs-lookup"><span data-stu-id="d2454-115">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2454-116">Relações</span><span class="sxs-lookup"><span data-stu-id="d2454-116">Relationships</span></span>
<span data-ttu-id="d2454-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2454-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d2454-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2454-118">JSON Representation</span></span>
<span data-ttu-id="d2454-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2454-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```





