---
title: tipo de recurso managedDeviceReportedApp
description: Dados de aplicativo para relatórios
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2f4549ac255913973610e3b09d41b2299229a309
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970126"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="83df2-103">tipo de recurso managedDeviceReportedApp</span><span class="sxs-lookup"><span data-stu-id="83df2-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="83df2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="83df2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83df2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83df2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83df2-106">Dados de aplicativo para relatórios</span><span class="sxs-lookup"><span data-stu-id="83df2-106">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="83df2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83df2-107">Properties</span></span>
|<span data-ttu-id="83df2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83df2-108">Property</span></span>|<span data-ttu-id="83df2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="83df2-109">Type</span></span>|<span data-ttu-id="83df2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="83df2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83df2-111">appId</span><span class="sxs-lookup"><span data-stu-id="83df2-111">appId</span></span>|<span data-ttu-id="83df2-112">String</span><span class="sxs-lookup"><span data-stu-id="83df2-112">String</span></span>|<span data-ttu-id="83df2-113">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="83df2-113">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="83df2-114">Relações</span><span class="sxs-lookup"><span data-stu-id="83df2-114">Relationships</span></span>
<span data-ttu-id="83df2-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="83df2-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83df2-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83df2-116">JSON Representation</span></span>
<span data-ttu-id="83df2-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83df2-117">Here is a JSON representation of the resource.</span></span>
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





