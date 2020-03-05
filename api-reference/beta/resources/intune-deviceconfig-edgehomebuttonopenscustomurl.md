---
title: tipo de recurso edgeHomeButtonOpensCustomURL
description: Mostrar o botão página inicial; clicar no botão página inicial carrega uma URL específica.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 60184022f219eba09f205121721b48fd6675d8c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530060"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="b1708-103">tipo de recurso edgeHomeButtonOpensCustomURL</span><span class="sxs-lookup"><span data-stu-id="b1708-103">edgeHomeButtonOpensCustomURL resource type</span></span>

<span data-ttu-id="b1708-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b1708-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1708-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b1708-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1708-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1708-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1708-107">Mostrar o botão página inicial; clicar no botão página inicial carrega uma URL específica.</span><span class="sxs-lookup"><span data-stu-id="b1708-107">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="b1708-108">Herda de [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1708-108">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b1708-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1708-109">Properties</span></span>
|<span data-ttu-id="b1708-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1708-110">Property</span></span>|<span data-ttu-id="b1708-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1708-111">Type</span></span>|<span data-ttu-id="b1708-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1708-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1708-113">homeButtonCustomURL</span><span class="sxs-lookup"><span data-stu-id="b1708-113">homeButtonCustomURL</span></span>|<span data-ttu-id="b1708-114">String</span><span class="sxs-lookup"><span data-stu-id="b1708-114">String</span></span>|<span data-ttu-id="b1708-115">A URL específica a ser carregada.</span><span class="sxs-lookup"><span data-stu-id="b1708-115">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1708-116">Relações</span><span class="sxs-lookup"><span data-stu-id="b1708-116">Relationships</span></span>
<span data-ttu-id="b1708-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b1708-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1708-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1708-118">JSON Representation</span></span>
<span data-ttu-id="b1708-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1708-119">Here is a JSON representation of the resource.</span></span>
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



