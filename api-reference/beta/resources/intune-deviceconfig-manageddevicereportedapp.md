---
title: tipo de recurso managedDeviceReportedApp
description: Dados de aplicativo para relatórios
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b243cbc5c3c06de6af3e2e0f1263b589edf86f48
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801166"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="823ae-103">tipo de recurso managedDeviceReportedApp</span><span class="sxs-lookup"><span data-stu-id="823ae-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="823ae-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="823ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="823ae-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="823ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="823ae-106">Dados de aplicativo para relatórios</span><span class="sxs-lookup"><span data-stu-id="823ae-106">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="823ae-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="823ae-107">Properties</span></span>
|<span data-ttu-id="823ae-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="823ae-108">Property</span></span>|<span data-ttu-id="823ae-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="823ae-109">Type</span></span>|<span data-ttu-id="823ae-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="823ae-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="823ae-111">appId</span><span class="sxs-lookup"><span data-stu-id="823ae-111">appId</span></span>|<span data-ttu-id="823ae-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="823ae-112">String</span></span>|<span data-ttu-id="823ae-113">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="823ae-113">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="823ae-114">Relações</span><span class="sxs-lookup"><span data-stu-id="823ae-114">Relationships</span></span>
<span data-ttu-id="823ae-115">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="823ae-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="823ae-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="823ae-116">JSON Representation</span></span>
<span data-ttu-id="823ae-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="823ae-117">Here is a JSON representation of the resource.</span></span>
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





