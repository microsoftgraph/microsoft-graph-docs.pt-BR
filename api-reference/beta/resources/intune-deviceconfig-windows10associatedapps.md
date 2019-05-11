---
title: tipo de recurso windows10AssociatedApps
description: Definição de aplicativo associado ao Windows 10.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fca7f8876ba0ea455d2bd7f537fe162f125e1dc9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944380"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="d5780-103">tipo de recurso windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="d5780-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="d5780-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d5780-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5780-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d5780-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5780-106">Definição de aplicativo associado ao Windows 10.</span><span class="sxs-lookup"><span data-stu-id="d5780-106">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="d5780-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5780-107">Properties</span></span>
|<span data-ttu-id="d5780-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5780-108">Property</span></span>|<span data-ttu-id="d5780-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5780-109">Type</span></span>|<span data-ttu-id="d5780-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5780-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5780-111">appType</span><span class="sxs-lookup"><span data-stu-id="d5780-111">appType</span></span>|[<span data-ttu-id="d5780-112">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="d5780-112">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="d5780-113">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d5780-113">Application type.</span></span> <span data-ttu-id="d5780-114">Os valores possíveis são: `desktop` e `universal`.</span><span class="sxs-lookup"><span data-stu-id="d5780-114">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="d5780-115">identificador</span><span class="sxs-lookup"><span data-stu-id="d5780-115">identifier</span></span>|<span data-ttu-id="d5780-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5780-116">String</span></span>|<span data-ttu-id="d5780-117">Identificação.</span><span class="sxs-lookup"><span data-stu-id="d5780-117">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5780-118">Relações</span><span class="sxs-lookup"><span data-stu-id="d5780-118">Relationships</span></span>
<span data-ttu-id="d5780-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5780-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5780-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5780-120">JSON Representation</span></span>
<span data-ttu-id="d5780-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5780-121">Here is a JSON representation of the resource.</span></span>
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




