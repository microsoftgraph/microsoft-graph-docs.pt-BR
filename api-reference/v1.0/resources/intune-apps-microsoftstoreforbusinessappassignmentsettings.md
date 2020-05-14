---
title: tipo de recurso microsoftStoreForBusinessAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dbfb271e8cfb0d019a0e127d1ad81ee033544a17
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "43457887"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="2bb82-103">tipo de recurso microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="2bb82-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

<span data-ttu-id="2bb82-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bb82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2bb82-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2bb82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bb82-106">Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.</span><span class="sxs-lookup"><span data-stu-id="2bb82-106">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="2bb82-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="2bb82-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2bb82-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2bb82-108">Properties</span></span>
|<span data-ttu-id="2bb82-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2bb82-109">Property</span></span>|<span data-ttu-id="2bb82-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bb82-110">Type</span></span>|<span data-ttu-id="2bb82-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bb82-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bb82-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="2bb82-112">useDeviceContext</span></span>|<span data-ttu-id="2bb82-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="2bb82-113">Boolean</span></span>|<span data-ttu-id="2bb82-114">Se é para usar ou não o contexto de execução do dispositivo em aplicativo móvel da Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="2bb82-114">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2bb82-115">Relações</span><span class="sxs-lookup"><span data-stu-id="2bb82-115">Relationships</span></span>
<span data-ttu-id="2bb82-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2bb82-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2bb82-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2bb82-117">JSON Representation</span></span>
<span data-ttu-id="2bb82-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2bb82-118">Here is a JSON representation of the resource.</span></span>
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







