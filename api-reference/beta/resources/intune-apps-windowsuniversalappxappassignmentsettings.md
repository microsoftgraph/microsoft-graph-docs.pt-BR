---
title: tipo de recurso de windowsUniversalAppXAppAssignmentSettings
description: Contém propriedades usadas durante a atribuição de um aplicativo móvel do AppX universais do Windows a um grupo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 27755a483be44584aeb82166f56e825df79f8eaa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400715"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="e59ae-103">tipo de recurso de windowsUniversalAppXAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="e59ae-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="e59ae-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e59ae-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e59ae-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e59ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e59ae-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e59ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e59ae-107">Contém propriedades usadas durante a atribuição de um aplicativo móvel do AppX universais do Windows a um grupo.</span><span class="sxs-lookup"><span data-stu-id="e59ae-107">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>


<span data-ttu-id="e59ae-108">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e59ae-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e59ae-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e59ae-109">Properties</span></span>
|<span data-ttu-id="e59ae-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e59ae-110">Property</span></span>|<span data-ttu-id="e59ae-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e59ae-111">Type</span></span>|<span data-ttu-id="e59ae-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e59ae-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e59ae-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="e59ae-113">useDeviceContext</span></span>|<span data-ttu-id="e59ae-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="e59ae-114">Boolean</span></span>|<span data-ttu-id="e59ae-115">Se deseja ou não usar o contexto de execução do dispositivo para aplicativos móveis de AppX Universal do Windows.</span><span class="sxs-lookup"><span data-stu-id="e59ae-115">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e59ae-116">Relações</span><span class="sxs-lookup"><span data-stu-id="e59ae-116">Relationships</span></span>
<span data-ttu-id="e59ae-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e59ae-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e59ae-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e59ae-118">JSON Representation</span></span>
<span data-ttu-id="e59ae-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e59ae-119">Here is a JSON representation of the resource.</span></span>
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




