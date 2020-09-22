---
title: tipo de recurso edgeHomeButtonOpensCustomURL
description: Mostrar o botão página inicial; clicar no botão página inicial carrega uma URL específica.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4779de3f0a6e53b8056a42e1df511ea176dd6378
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058232"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="3ff83-103">tipo de recurso edgeHomeButtonOpensCustomURL</span><span class="sxs-lookup"><span data-stu-id="3ff83-103">edgeHomeButtonOpensCustomURL resource type</span></span>

<span data-ttu-id="3ff83-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ff83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ff83-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3ff83-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ff83-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3ff83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ff83-107">Mostrar o botão página inicial; clicar no botão página inicial carrega uma URL específica.</span><span class="sxs-lookup"><span data-stu-id="3ff83-107">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="3ff83-108">Herda de [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ff83-108">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3ff83-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ff83-109">Properties</span></span>
|<span data-ttu-id="3ff83-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ff83-110">Property</span></span>|<span data-ttu-id="3ff83-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ff83-111">Type</span></span>|<span data-ttu-id="3ff83-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ff83-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ff83-113">homeButtonCustomURL</span><span class="sxs-lookup"><span data-stu-id="3ff83-113">homeButtonCustomURL</span></span>|<span data-ttu-id="3ff83-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ff83-114">String</span></span>|<span data-ttu-id="3ff83-115">A URL específica a ser carregada.</span><span class="sxs-lookup"><span data-stu-id="3ff83-115">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ff83-116">Relações</span><span class="sxs-lookup"><span data-stu-id="3ff83-116">Relationships</span></span>
<span data-ttu-id="3ff83-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3ff83-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ff83-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ff83-118">JSON Representation</span></span>
<span data-ttu-id="3ff83-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3ff83-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeHomeButtonOpensCustomURL"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeHomeButtonOpensCustomURL",
  "homeButtonCustomURL": "String"
}
```






