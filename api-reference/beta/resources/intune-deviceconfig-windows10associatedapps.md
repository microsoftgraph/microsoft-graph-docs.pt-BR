---
title: tipo de recurso windows10AssociatedApps
description: Definição de aplicativo associado ao Windows 10.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ecdea1d1493388c1fab3037d49b41f5f3388e3c0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985913"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="9c283-103">tipo de recurso windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="9c283-103">windows10AssociatedApps resource type</span></span>

<span data-ttu-id="9c283-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c283-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c283-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9c283-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c283-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9c283-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c283-107">Definição de aplicativo associado ao Windows 10.</span><span class="sxs-lookup"><span data-stu-id="9c283-107">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="9c283-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c283-108">Properties</span></span>
|<span data-ttu-id="9c283-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c283-109">Property</span></span>|<span data-ttu-id="9c283-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c283-110">Type</span></span>|<span data-ttu-id="9c283-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c283-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c283-112">appType</span><span class="sxs-lookup"><span data-stu-id="9c283-112">appType</span></span>|[<span data-ttu-id="9c283-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="9c283-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="9c283-114">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9c283-114">Application type.</span></span> <span data-ttu-id="9c283-115">Os valores possíveis são: `desktop` e `universal`.</span><span class="sxs-lookup"><span data-stu-id="9c283-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="9c283-116">identificador</span><span class="sxs-lookup"><span data-stu-id="9c283-116">identifier</span></span>|<span data-ttu-id="9c283-117">String</span><span class="sxs-lookup"><span data-stu-id="9c283-117">String</span></span>|<span data-ttu-id="9c283-118">Identificação.</span><span class="sxs-lookup"><span data-stu-id="9c283-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c283-119">Relações</span><span class="sxs-lookup"><span data-stu-id="9c283-119">Relationships</span></span>
<span data-ttu-id="9c283-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c283-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c283-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c283-121">JSON Representation</span></span>
<span data-ttu-id="9c283-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c283-122">Here is a JSON representation of the resource.</span></span>
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






