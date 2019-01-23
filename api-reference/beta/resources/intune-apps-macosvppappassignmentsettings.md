---
title: tipo de recurso de macOsVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do Mac VPP a um grupo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0927277b11416da001ad826200bf4ec841341118
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431312"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="93125-103">tipo de recurso de macOsVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="93125-103">macOsVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="93125-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="93125-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="93125-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="93125-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="93125-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="93125-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93125-107">Contém propriedades usadas para atribuir um aplicativo móvel do Mac VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="93125-107">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="93125-108">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="93125-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="93125-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93125-109">Properties</span></span>
|<span data-ttu-id="93125-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93125-110">Property</span></span>|<span data-ttu-id="93125-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="93125-111">Type</span></span>|<span data-ttu-id="93125-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="93125-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93125-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="93125-113">useDeviceLicensing</span></span>|<span data-ttu-id="93125-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="93125-114">Boolean</span></span>|<span data-ttu-id="93125-115">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="93125-115">Whether or not to use device licensing.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93125-116">Relações</span><span class="sxs-lookup"><span data-stu-id="93125-116">Relationships</span></span>
<span data-ttu-id="93125-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="93125-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93125-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93125-118">JSON Representation</span></span>
<span data-ttu-id="93125-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93125-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignmentSettings",
  "useDeviceLicensing": true
}
```




