---
title: tipo de recurso windows10AssociatedApps
description: Definição de aplicativo associado ao Windows 10.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2860414d2cff95adb02302d4f375784d1e1a6063
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49307658"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="8fc7e-103">tipo de recurso windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="8fc7e-103">windows10AssociatedApps resource type</span></span>

<span data-ttu-id="8fc7e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fc7e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8fc7e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8fc7e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fc7e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8fc7e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fc7e-107">Definição de aplicativo associado ao Windows 10.</span><span class="sxs-lookup"><span data-stu-id="8fc7e-107">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="8fc7e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8fc7e-108">Properties</span></span>
|<span data-ttu-id="8fc7e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8fc7e-109">Property</span></span>|<span data-ttu-id="8fc7e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8fc7e-110">Type</span></span>|<span data-ttu-id="8fc7e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fc7e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fc7e-112">appType</span><span class="sxs-lookup"><span data-stu-id="8fc7e-112">appType</span></span>|[<span data-ttu-id="8fc7e-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="8fc7e-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="8fc7e-114">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8fc7e-114">Application type.</span></span> <span data-ttu-id="8fc7e-115">Os valores possíveis são: `desktop` e `universal`.</span><span class="sxs-lookup"><span data-stu-id="8fc7e-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="8fc7e-116">identificador</span><span class="sxs-lookup"><span data-stu-id="8fc7e-116">identifier</span></span>|<span data-ttu-id="8fc7e-117">String</span><span class="sxs-lookup"><span data-stu-id="8fc7e-117">String</span></span>|<span data-ttu-id="8fc7e-118">Identificação.</span><span class="sxs-lookup"><span data-stu-id="8fc7e-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fc7e-119">Relações</span><span class="sxs-lookup"><span data-stu-id="8fc7e-119">Relationships</span></span>
<span data-ttu-id="8fc7e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8fc7e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8fc7e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8fc7e-121">JSON Representation</span></span>
<span data-ttu-id="8fc7e-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8fc7e-122">Here is a JSON representation of the resource.</span></span>
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




