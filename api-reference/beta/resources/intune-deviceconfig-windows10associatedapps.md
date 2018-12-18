---
title: tipo de recurso de windows10AssociatedApps
description: Definição de aplicativo do Windows 10 associados.
author: tfitzmac
ms.openlocfilehash: a990d3b1f9b2b33a1e98fd30f5dea4da7fbf4ae8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344825"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="7bd7b-103">tipo de recurso de windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="7bd7b-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="7bd7b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7bd7b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7bd7b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7bd7b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7bd7b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7bd7b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7bd7b-107">Definição de aplicativo do Windows 10 associados.</span><span class="sxs-lookup"><span data-stu-id="7bd7b-107">Windows 10 Associated Application definition.</span></span>
## <a name="properties"></a><span data-ttu-id="7bd7b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7bd7b-108">Properties</span></span>
|<span data-ttu-id="7bd7b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bd7b-109">Property</span></span>|<span data-ttu-id="7bd7b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bd7b-110">Type</span></span>|<span data-ttu-id="7bd7b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bd7b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bd7b-112">tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bd7b-112">appType</span></span>|[<span data-ttu-id="7bd7b-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="7bd7b-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="7bd7b-114">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7bd7b-114">Application type.</span></span> <span data-ttu-id="7bd7b-115">Os valores possíveis são: `desktop` e `universal`.</span><span class="sxs-lookup"><span data-stu-id="7bd7b-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="7bd7b-116">identificador</span><span class="sxs-lookup"><span data-stu-id="7bd7b-116">identifier</span></span>|<span data-ttu-id="7bd7b-117">String</span><span class="sxs-lookup"><span data-stu-id="7bd7b-117">String</span></span>|<span data-ttu-id="7bd7b-118">Identificador.</span><span class="sxs-lookup"><span data-stu-id="7bd7b-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bd7b-119">Relações</span><span class="sxs-lookup"><span data-stu-id="7bd7b-119">Relationships</span></span>
<span data-ttu-id="7bd7b-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7bd7b-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7bd7b-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7bd7b-121">JSON Representation</span></span>
<span data-ttu-id="7bd7b-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7bd7b-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AssociatedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AssociatedApps",
  "appType": "String",
  "identifier": "String"
}
```





