---
title: tipo de recurso managedDeviceReportedApp
description: Dados de aplicativo para relatórios
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: beeb1b8919e6e8caec0a055a5520c4a71c131e90
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010182"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="0b731-103">tipo de recurso managedDeviceReportedApp</span><span class="sxs-lookup"><span data-stu-id="0b731-103">managedDeviceReportedApp resource type</span></span>

<span data-ttu-id="0b731-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b731-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b731-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0b731-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b731-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0b731-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b731-107">Dados de aplicativo para relatórios</span><span class="sxs-lookup"><span data-stu-id="0b731-107">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="0b731-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b731-108">Properties</span></span>
|<span data-ttu-id="0b731-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b731-109">Property</span></span>|<span data-ttu-id="0b731-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b731-110">Type</span></span>|<span data-ttu-id="0b731-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b731-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b731-112">appId</span><span class="sxs-lookup"><span data-stu-id="0b731-112">appId</span></span>|<span data-ttu-id="0b731-113">String</span><span class="sxs-lookup"><span data-stu-id="0b731-113">String</span></span>|<span data-ttu-id="0b731-114">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b731-114">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b731-115">Relações</span><span class="sxs-lookup"><span data-stu-id="0b731-115">Relationships</span></span>
<span data-ttu-id="0b731-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b731-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b731-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b731-117">JSON Representation</span></span>
<span data-ttu-id="0b731-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b731-118">Here is a JSON representation of the resource.</span></span>
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






