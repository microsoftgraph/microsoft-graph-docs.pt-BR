---
title: tipo de recurso de windows10AssociatedApps
description: Definição de aplicativo do Windows 10 associados.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d1f6363027ae46263146efdbf3f5ac5254afcd93
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911907"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="4872e-103">tipo de recurso de windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="4872e-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="4872e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4872e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4872e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4872e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4872e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4872e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4872e-107">Definição de aplicativo do Windows 10 associados.</span><span class="sxs-lookup"><span data-stu-id="4872e-107">Windows 10 Associated Application definition.</span></span>
## <a name="properties"></a><span data-ttu-id="4872e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4872e-108">Properties</span></span>
|<span data-ttu-id="4872e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4872e-109">Property</span></span>|<span data-ttu-id="4872e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4872e-110">Type</span></span>|<span data-ttu-id="4872e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4872e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4872e-112">tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="4872e-112">appType</span></span>|[<span data-ttu-id="4872e-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="4872e-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="4872e-114">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4872e-114">Application type.</span></span> <span data-ttu-id="4872e-115">Os valores possíveis são: `desktop` e `universal`.</span><span class="sxs-lookup"><span data-stu-id="4872e-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="4872e-116">identificador</span><span class="sxs-lookup"><span data-stu-id="4872e-116">identifier</span></span>|<span data-ttu-id="4872e-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4872e-117">String</span></span>|<span data-ttu-id="4872e-118">Identificador.</span><span class="sxs-lookup"><span data-stu-id="4872e-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4872e-119">Relações</span><span class="sxs-lookup"><span data-stu-id="4872e-119">Relationships</span></span>
<span data-ttu-id="4872e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4872e-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4872e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4872e-121">JSON Representation</span></span>
<span data-ttu-id="4872e-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4872e-122">Here is a JSON representation of the resource.</span></span>
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





