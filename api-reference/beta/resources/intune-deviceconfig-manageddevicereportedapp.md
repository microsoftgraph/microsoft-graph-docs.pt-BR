---
title: tipo de recurso de managedDeviceReportedApp
description: Dados de aplicativo para relatórios
ms.openlocfilehash: 820269422891e01352a7f605d62147a84facea67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033973"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="9dd88-103">tipo de recurso de managedDeviceReportedApp</span><span class="sxs-lookup"><span data-stu-id="9dd88-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="9dd88-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9dd88-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9dd88-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9dd88-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9dd88-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9dd88-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9dd88-107">Dados de aplicativo para relatórios</span><span class="sxs-lookup"><span data-stu-id="9dd88-107">Application data for reporting</span></span>
## <a name="properties"></a><span data-ttu-id="9dd88-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9dd88-108">Properties</span></span>
|<span data-ttu-id="9dd88-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9dd88-109">Property</span></span>|<span data-ttu-id="9dd88-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9dd88-110">Type</span></span>|<span data-ttu-id="9dd88-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9dd88-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dd88-112">appId</span><span class="sxs-lookup"><span data-stu-id="9dd88-112">appId</span></span>|<span data-ttu-id="9dd88-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9dd88-113">String</span></span>|<span data-ttu-id="9dd88-114">O aplicativo ou identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="9dd88-114">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="9dd88-115">Relações</span><span class="sxs-lookup"><span data-stu-id="9dd88-115">Relationships</span></span>
<span data-ttu-id="9dd88-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9dd88-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9dd88-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9dd88-117">JSON Representation</span></span>
<span data-ttu-id="9dd88-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9dd88-118">Here is a JSON representation of the resource.</span></span>
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





