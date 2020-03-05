---
title: tipo de recurso managedDeviceReportedApp
description: Dados de aplicativo para relatórios
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ff42634a69ce9c7ea3c2e54e88401b8041348fc0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526045"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="544f1-103">tipo de recurso managedDeviceReportedApp</span><span class="sxs-lookup"><span data-stu-id="544f1-103">managedDeviceReportedApp resource type</span></span>

<span data-ttu-id="544f1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="544f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="544f1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="544f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="544f1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="544f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="544f1-107">Dados de aplicativo para relatórios</span><span class="sxs-lookup"><span data-stu-id="544f1-107">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="544f1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="544f1-108">Properties</span></span>
|<span data-ttu-id="544f1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="544f1-109">Property</span></span>|<span data-ttu-id="544f1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="544f1-110">Type</span></span>|<span data-ttu-id="544f1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="544f1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="544f1-112">appId</span><span class="sxs-lookup"><span data-stu-id="544f1-112">appId</span></span>|<span data-ttu-id="544f1-113">String</span><span class="sxs-lookup"><span data-stu-id="544f1-113">String</span></span>|<span data-ttu-id="544f1-114">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="544f1-114">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="544f1-115">Relações</span><span class="sxs-lookup"><span data-stu-id="544f1-115">Relationships</span></span>
<span data-ttu-id="544f1-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="544f1-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="544f1-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="544f1-117">JSON Representation</span></span>
<span data-ttu-id="544f1-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="544f1-118">Here is a JSON representation of the resource.</span></span>
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



