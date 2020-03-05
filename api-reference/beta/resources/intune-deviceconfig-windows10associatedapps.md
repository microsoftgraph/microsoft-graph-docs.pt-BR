---
title: tipo de recurso windows10AssociatedApps
description: Definição de aplicativo associado ao Windows 10.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ba372cd3e8f67371adac9f92da92da4c7efe2a28
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525688"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="69592-103">tipo de recurso windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="69592-103">windows10AssociatedApps resource type</span></span>

<span data-ttu-id="69592-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="69592-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69592-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="69592-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69592-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="69592-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69592-107">Definição de aplicativo associado ao Windows 10.</span><span class="sxs-lookup"><span data-stu-id="69592-107">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="69592-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69592-108">Properties</span></span>
|<span data-ttu-id="69592-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69592-109">Property</span></span>|<span data-ttu-id="69592-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="69592-110">Type</span></span>|<span data-ttu-id="69592-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="69592-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69592-112">appType</span><span class="sxs-lookup"><span data-stu-id="69592-112">appType</span></span>|[<span data-ttu-id="69592-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="69592-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="69592-114">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="69592-114">Application type.</span></span> <span data-ttu-id="69592-115">Os valores possíveis são: `desktop` e `universal`.</span><span class="sxs-lookup"><span data-stu-id="69592-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="69592-116">identificador</span><span class="sxs-lookup"><span data-stu-id="69592-116">identifier</span></span>|<span data-ttu-id="69592-117">String</span><span class="sxs-lookup"><span data-stu-id="69592-117">String</span></span>|<span data-ttu-id="69592-118">Identificação.</span><span class="sxs-lookup"><span data-stu-id="69592-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69592-119">Relações</span><span class="sxs-lookup"><span data-stu-id="69592-119">Relationships</span></span>
<span data-ttu-id="69592-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="69592-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69592-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69592-121">JSON Representation</span></span>
<span data-ttu-id="69592-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69592-122">Here is a JSON representation of the resource.</span></span>
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



