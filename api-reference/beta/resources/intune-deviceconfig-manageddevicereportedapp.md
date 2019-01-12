---
title: tipo de recurso de managedDeviceReportedApp
description: Dados de aplicativo para relatórios
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8aa9a4d825e2333e135a676fa1eeb88e7cfe079c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942973"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="75332-103">tipo de recurso de managedDeviceReportedApp</span><span class="sxs-lookup"><span data-stu-id="75332-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="75332-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="75332-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75332-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="75332-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="75332-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="75332-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75332-107">Dados de aplicativo para relatórios</span><span class="sxs-lookup"><span data-stu-id="75332-107">Application data for reporting</span></span>
## <a name="properties"></a><span data-ttu-id="75332-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75332-108">Properties</span></span>
|<span data-ttu-id="75332-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75332-109">Property</span></span>|<span data-ttu-id="75332-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="75332-110">Type</span></span>|<span data-ttu-id="75332-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="75332-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75332-112">appId</span><span class="sxs-lookup"><span data-stu-id="75332-112">appId</span></span>|<span data-ttu-id="75332-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75332-113">String</span></span>|<span data-ttu-id="75332-114">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="75332-114">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="75332-115">Relações</span><span class="sxs-lookup"><span data-stu-id="75332-115">Relationships</span></span>
<span data-ttu-id="75332-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="75332-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="75332-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75332-117">JSON Representation</span></span>
<span data-ttu-id="75332-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="75332-118">Here is a JSON representation of the resource.</span></span>
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





