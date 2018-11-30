---
title: tipo de recurso de windowsUniversalAppXAppAssignmentSettings
description: Contém propriedades usadas durante a atribuição de um aplicativo móvel do AppX universais do Windows a um grupo.
ms.openlocfilehash: 9694ab347be6edd1446df8aa7b46fb3652aee589
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037075"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="6ea0c-103">tipo de recurso de windowsUniversalAppXAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="6ea0c-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="6ea0c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6ea0c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ea0c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6ea0c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ea0c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6ea0c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ea0c-107">Contém propriedades usadas durante a atribuição de um aplicativo móvel do AppX universais do Windows a um grupo.</span><span class="sxs-lookup"><span data-stu-id="6ea0c-107">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>

<span data-ttu-id="6ea0c-108">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="6ea0c-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6ea0c-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6ea0c-109">Properties</span></span>
|<span data-ttu-id="6ea0c-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ea0c-110">Property</span></span>|<span data-ttu-id="6ea0c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ea0c-111">Type</span></span>|<span data-ttu-id="6ea0c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ea0c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ea0c-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="6ea0c-113">useDeviceContext</span></span>|<span data-ttu-id="6ea0c-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ea0c-114">Boolean</span></span>|<span data-ttu-id="6ea0c-115">Se deseja ou não usar o contexto de execução do dispositivo para aplicativos móveis de AppX Universal do Windows.</span><span class="sxs-lookup"><span data-stu-id="6ea0c-115">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ea0c-116">Relações</span><span class="sxs-lookup"><span data-stu-id="6ea0c-116">Relationships</span></span>
<span data-ttu-id="6ea0c-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6ea0c-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6ea0c-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6ea0c-118">JSON Representation</span></span>
<span data-ttu-id="6ea0c-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6ea0c-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUniversalAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```





