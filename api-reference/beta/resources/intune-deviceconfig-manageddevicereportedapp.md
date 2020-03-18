---
title: tipo de recurso managedDeviceReportedApp
description: Dados de aplicativo para relatórios
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6704e4f2f8796be6c246d6deb6f5e0e8821ba411
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788608"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="7c83a-103">tipo de recurso managedDeviceReportedApp</span><span class="sxs-lookup"><span data-stu-id="7c83a-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="7c83a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7c83a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c83a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c83a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c83a-106">Dados de aplicativo para relatórios</span><span class="sxs-lookup"><span data-stu-id="7c83a-106">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="7c83a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7c83a-107">Properties</span></span>
|<span data-ttu-id="7c83a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c83a-108">Property</span></span>|<span data-ttu-id="7c83a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c83a-109">Type</span></span>|<span data-ttu-id="7c83a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c83a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c83a-111">appId</span><span class="sxs-lookup"><span data-stu-id="7c83a-111">appId</span></span>|<span data-ttu-id="7c83a-112">String</span><span class="sxs-lookup"><span data-stu-id="7c83a-112">String</span></span>|<span data-ttu-id="7c83a-113">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c83a-113">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c83a-114">Relações</span><span class="sxs-lookup"><span data-stu-id="7c83a-114">Relationships</span></span>
<span data-ttu-id="7c83a-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7c83a-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c83a-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7c83a-116">JSON Representation</span></span>
<span data-ttu-id="7c83a-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7c83a-117">Here is a JSON representation of the resource.</span></span>
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



