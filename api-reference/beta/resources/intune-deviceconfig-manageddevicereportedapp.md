---
title: tipo de recurso managedDeviceReportedApp
description: Dados de aplicativo para relatórios
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6561a6cee5a02f46c3347a1919c93c3807250fa8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368822"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="21ecc-103">tipo de recurso managedDeviceReportedApp</span><span class="sxs-lookup"><span data-stu-id="21ecc-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="21ecc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="21ecc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21ecc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21ecc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21ecc-106">Dados de aplicativo para relatórios</span><span class="sxs-lookup"><span data-stu-id="21ecc-106">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="21ecc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21ecc-107">Properties</span></span>
|<span data-ttu-id="21ecc-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21ecc-108">Property</span></span>|<span data-ttu-id="21ecc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="21ecc-109">Type</span></span>|<span data-ttu-id="21ecc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="21ecc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21ecc-111">appId</span><span class="sxs-lookup"><span data-stu-id="21ecc-111">appId</span></span>|<span data-ttu-id="21ecc-112">String</span><span class="sxs-lookup"><span data-stu-id="21ecc-112">String</span></span>|<span data-ttu-id="21ecc-113">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="21ecc-113">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="21ecc-114">Relações</span><span class="sxs-lookup"><span data-stu-id="21ecc-114">Relationships</span></span>
<span data-ttu-id="21ecc-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="21ecc-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21ecc-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21ecc-116">JSON Representation</span></span>
<span data-ttu-id="21ecc-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21ecc-117">Here is a JSON representation of the resource.</span></span>
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



