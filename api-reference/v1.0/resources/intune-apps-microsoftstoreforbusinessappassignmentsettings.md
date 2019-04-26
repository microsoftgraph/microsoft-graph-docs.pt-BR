---
title: tipo de recurso microsoftStoreForBusinessAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c1aed45ba54abdcb25f5436beeb2a03f53b9dbae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558115"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="592a4-103">tipo de recurso microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="592a4-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="592a4-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="592a4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="592a4-105">Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.</span><span class="sxs-lookup"><span data-stu-id="592a4-105">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="592a4-106">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="592a4-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="592a4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="592a4-107">Properties</span></span>
|<span data-ttu-id="592a4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="592a4-108">Property</span></span>|<span data-ttu-id="592a4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="592a4-109">Type</span></span>|<span data-ttu-id="592a4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="592a4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="592a4-111">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="592a4-111">useDeviceContext</span></span>|<span data-ttu-id="592a4-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="592a4-112">Boolean</span></span>|<span data-ttu-id="592a4-113">Se é para usar ou não o contexto de execução do dispositivo em aplicativo móvel da Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="592a4-113">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="592a4-114">Relações</span><span class="sxs-lookup"><span data-stu-id="592a4-114">Relationships</span></span>
<span data-ttu-id="592a4-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="592a4-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="592a4-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="592a4-116">JSON Representation</span></span>
<span data-ttu-id="592a4-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="592a4-117">Here is a JSON representation of the resource.</span></span>
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



