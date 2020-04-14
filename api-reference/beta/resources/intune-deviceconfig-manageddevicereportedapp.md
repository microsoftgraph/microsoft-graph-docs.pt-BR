---
title: tipo de recurso managedDeviceReportedApp
description: Dados de aplicativo para relatórios
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d3e0fa86d6057cf5521f4adb1ecf098e302ae018
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437248"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="93a8d-103">tipo de recurso managedDeviceReportedApp</span><span class="sxs-lookup"><span data-stu-id="93a8d-103">managedDeviceReportedApp resource type</span></span>

<span data-ttu-id="93a8d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93a8d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93a8d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="93a8d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93a8d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="93a8d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93a8d-107">Dados de aplicativo para relatórios</span><span class="sxs-lookup"><span data-stu-id="93a8d-107">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="93a8d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93a8d-108">Properties</span></span>
|<span data-ttu-id="93a8d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93a8d-109">Property</span></span>|<span data-ttu-id="93a8d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="93a8d-110">Type</span></span>|<span data-ttu-id="93a8d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="93a8d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93a8d-112">appId</span><span class="sxs-lookup"><span data-stu-id="93a8d-112">appId</span></span>|<span data-ttu-id="93a8d-113">String</span><span class="sxs-lookup"><span data-stu-id="93a8d-113">String</span></span>|<span data-ttu-id="93a8d-114">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="93a8d-114">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="93a8d-115">Relações</span><span class="sxs-lookup"><span data-stu-id="93a8d-115">Relationships</span></span>
<span data-ttu-id="93a8d-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="93a8d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93a8d-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93a8d-117">JSON Representation</span></span>
<span data-ttu-id="93a8d-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93a8d-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceReportedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceReportedApp",
  "appId": "String"
}
```



