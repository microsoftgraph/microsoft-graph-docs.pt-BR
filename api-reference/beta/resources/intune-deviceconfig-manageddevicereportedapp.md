---
title: tipo de recurso managedDeviceReportedApp
description: Dados de aplicativo para relatórios
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76317a14d05ad1e4a949485f2ae63e00b1e91b81
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944940"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="409ed-103">tipo de recurso managedDeviceReportedApp</span><span class="sxs-lookup"><span data-stu-id="409ed-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="409ed-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="409ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="409ed-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="409ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="409ed-106">Dados de aplicativo para relatórios</span><span class="sxs-lookup"><span data-stu-id="409ed-106">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="409ed-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="409ed-107">Properties</span></span>
|<span data-ttu-id="409ed-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="409ed-108">Property</span></span>|<span data-ttu-id="409ed-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="409ed-109">Type</span></span>|<span data-ttu-id="409ed-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="409ed-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="409ed-111">appId</span><span class="sxs-lookup"><span data-stu-id="409ed-111">appId</span></span>|<span data-ttu-id="409ed-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="409ed-112">String</span></span>|<span data-ttu-id="409ed-113">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="409ed-113">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="409ed-114">Relações</span><span class="sxs-lookup"><span data-stu-id="409ed-114">Relationships</span></span>
<span data-ttu-id="409ed-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="409ed-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="409ed-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="409ed-116">JSON Representation</span></span>
<span data-ttu-id="409ed-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="409ed-117">Here is a JSON representation of the resource.</span></span>
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




