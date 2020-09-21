---
title: tipo de recurso microsoftStoreForBusinessAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de6faaf42df24ae89f8d0dd514e1beb4d1b6cb25
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070776"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="affaa-103">tipo de recurso microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="affaa-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

<span data-ttu-id="affaa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="affaa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="affaa-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="affaa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="affaa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="affaa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="affaa-107">Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.</span><span class="sxs-lookup"><span data-stu-id="affaa-107">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="affaa-108">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="affaa-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="affaa-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="affaa-109">Properties</span></span>
|<span data-ttu-id="affaa-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="affaa-110">Property</span></span>|<span data-ttu-id="affaa-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="affaa-111">Type</span></span>|<span data-ttu-id="affaa-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="affaa-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="affaa-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="affaa-113">useDeviceContext</span></span>|<span data-ttu-id="affaa-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="affaa-114">Boolean</span></span>|<span data-ttu-id="affaa-115">Se é para usar ou não o contexto de execução do dispositivo em aplicativo móvel da Microsoft Store para Empresas.</span><span class="sxs-lookup"><span data-stu-id="affaa-115">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="affaa-116">Relações</span><span class="sxs-lookup"><span data-stu-id="affaa-116">Relationships</span></span>
<span data-ttu-id="affaa-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="affaa-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="affaa-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="affaa-118">JSON Representation</span></span>
<span data-ttu-id="affaa-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="affaa-119">Here is a JSON representation of the resource.</span></span>
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






