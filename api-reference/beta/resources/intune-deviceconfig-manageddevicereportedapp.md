---
title: tipo de recurso managedDeviceReportedApp
description: Dados de aplicativo para relatórios
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e028ec07142a7902ec02b2b8eeccdc9c378170d8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992021"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="be678-103">tipo de recurso managedDeviceReportedApp</span><span class="sxs-lookup"><span data-stu-id="be678-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="be678-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="be678-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be678-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="be678-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be678-106">Dados de aplicativo para relatórios</span><span class="sxs-lookup"><span data-stu-id="be678-106">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="be678-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="be678-107">Properties</span></span>
|<span data-ttu-id="be678-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be678-108">Property</span></span>|<span data-ttu-id="be678-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="be678-109">Type</span></span>|<span data-ttu-id="be678-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="be678-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be678-111">appId</span><span class="sxs-lookup"><span data-stu-id="be678-111">appId</span></span>|<span data-ttu-id="be678-112">String</span><span class="sxs-lookup"><span data-stu-id="be678-112">String</span></span>|<span data-ttu-id="be678-113">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="be678-113">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="be678-114">Relações</span><span class="sxs-lookup"><span data-stu-id="be678-114">Relationships</span></span>
<span data-ttu-id="be678-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="be678-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be678-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="be678-116">JSON Representation</span></span>
<span data-ttu-id="be678-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="be678-117">Here is a JSON representation of the resource.</span></span>
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





