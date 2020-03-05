---
title: tipo de recurso vpnRoute
description: Definição da rota VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4c383c539cf74bbbd4119294ea150394e37bf1a9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529289"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="775ca-103">tipo de recurso vpnRoute</span><span class="sxs-lookup"><span data-stu-id="775ca-103">vpnRoute resource type</span></span>

<span data-ttu-id="775ca-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="775ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="775ca-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="775ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="775ca-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="775ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="775ca-107">Definição da rota VPN.</span><span class="sxs-lookup"><span data-stu-id="775ca-107">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="775ca-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="775ca-108">Properties</span></span>
|<span data-ttu-id="775ca-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="775ca-109">Property</span></span>|<span data-ttu-id="775ca-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="775ca-110">Type</span></span>|<span data-ttu-id="775ca-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="775ca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="775ca-112">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="775ca-112">destinationPrefix</span></span>|<span data-ttu-id="775ca-113">String</span><span class="sxs-lookup"><span data-stu-id="775ca-113">String</span></span>|<span data-ttu-id="775ca-114">Prefixo de destino (endereço IPv4/V6).</span><span class="sxs-lookup"><span data-stu-id="775ca-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="775ca-115">prefixSize</span><span class="sxs-lookup"><span data-stu-id="775ca-115">prefixSize</span></span>|<span data-ttu-id="775ca-116">Int32</span><span class="sxs-lookup"><span data-stu-id="775ca-116">Int32</span></span>|<span data-ttu-id="775ca-117">Tamanho do prefixo.</span><span class="sxs-lookup"><span data-stu-id="775ca-117">Prefix size.</span></span> <span data-ttu-id="775ca-118">(1-32).</span><span class="sxs-lookup"><span data-stu-id="775ca-118">(1-32).</span></span> <span data-ttu-id="775ca-119">Valores válidos de 1 a 32</span><span class="sxs-lookup"><span data-stu-id="775ca-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="775ca-120">Relações</span><span class="sxs-lookup"><span data-stu-id="775ca-120">Relationships</span></span>
<span data-ttu-id="775ca-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="775ca-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="775ca-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="775ca-122">JSON Representation</span></span>
<span data-ttu-id="775ca-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="775ca-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnRoute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnRoute",
  "destinationPrefix": "String",
  "prefixSize": 1024
}
```



