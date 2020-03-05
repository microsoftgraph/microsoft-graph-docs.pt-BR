---
title: tipo de recurso microsoftStoreForBusinessAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bb2dc1fda4fdc903bd64d053ce377f4f5f203aa7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523629"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="303f9-103">tipo de recurso microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="303f9-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

<span data-ttu-id="303f9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="303f9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="303f9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="303f9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="303f9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="303f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="303f9-107">Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.</span><span class="sxs-lookup"><span data-stu-id="303f9-107">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="303f9-108">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="303f9-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="303f9-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="303f9-109">Properties</span></span>
|<span data-ttu-id="303f9-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="303f9-110">Property</span></span>|<span data-ttu-id="303f9-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="303f9-111">Type</span></span>|<span data-ttu-id="303f9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="303f9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="303f9-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="303f9-113">useDeviceContext</span></span>|<span data-ttu-id="303f9-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="303f9-114">Boolean</span></span>|<span data-ttu-id="303f9-115">Se é para usar ou não o contexto de execução do dispositivo em aplicativo móvel da Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="303f9-115">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="303f9-116">Relações</span><span class="sxs-lookup"><span data-stu-id="303f9-116">Relationships</span></span>
<span data-ttu-id="303f9-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="303f9-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="303f9-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="303f9-118">JSON Representation</span></span>
<span data-ttu-id="303f9-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="303f9-119">Here is a JSON representation of the resource.</span></span>
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



