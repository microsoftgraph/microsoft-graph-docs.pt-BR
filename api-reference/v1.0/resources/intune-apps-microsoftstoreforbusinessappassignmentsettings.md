---
title: tipo de recurso microsoftStoreForBusinessAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c42ea0ca8175b22d24061133a8c748f7225e2dd3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755130"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="e32ed-103">tipo de recurso microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="e32ed-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

<span data-ttu-id="e32ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e32ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e32ed-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e32ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e32ed-106">Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.</span><span class="sxs-lookup"><span data-stu-id="e32ed-106">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="e32ed-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e32ed-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e32ed-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e32ed-108">Properties</span></span>
|<span data-ttu-id="e32ed-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e32ed-109">Property</span></span>|<span data-ttu-id="e32ed-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e32ed-110">Type</span></span>|<span data-ttu-id="e32ed-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e32ed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e32ed-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="e32ed-112">useDeviceContext</span></span>|<span data-ttu-id="e32ed-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="e32ed-113">Boolean</span></span>|<span data-ttu-id="e32ed-114">Se é para usar ou não o contexto de execução do dispositivo em aplicativo móvel da Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="e32ed-114">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e32ed-115">Relações</span><span class="sxs-lookup"><span data-stu-id="e32ed-115">Relationships</span></span>
<span data-ttu-id="e32ed-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e32ed-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e32ed-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e32ed-117">JSON Representation</span></span>
<span data-ttu-id="e32ed-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e32ed-118">Here is a JSON representation of the resource.</span></span>
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




