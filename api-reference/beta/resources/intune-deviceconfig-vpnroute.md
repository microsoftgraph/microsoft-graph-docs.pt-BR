---
title: tipo de recurso de vpnRoute
description: Definição de rota da VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 628e2f384b06dece13da1595a4111a2d1022a673
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423017"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="c526b-103">tipo de recurso de vpnRoute</span><span class="sxs-lookup"><span data-stu-id="c526b-103">vpnRoute resource type</span></span>

> <span data-ttu-id="c526b-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c526b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c526b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c526b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c526b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c526b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c526b-107">Definição de rota da VPN.</span><span class="sxs-lookup"><span data-stu-id="c526b-107">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="c526b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c526b-108">Properties</span></span>
|<span data-ttu-id="c526b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c526b-109">Property</span></span>|<span data-ttu-id="c526b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c526b-110">Type</span></span>|<span data-ttu-id="c526b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c526b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c526b-112">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="c526b-112">destinationPrefix</span></span>|<span data-ttu-id="c526b-113">String</span><span class="sxs-lookup"><span data-stu-id="c526b-113">String</span></span>|<span data-ttu-id="c526b-114">Prefixo de destino (endereço IPv4/v6).</span><span class="sxs-lookup"><span data-stu-id="c526b-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="c526b-115">prefixSize</span><span class="sxs-lookup"><span data-stu-id="c526b-115">prefixSize</span></span>|<span data-ttu-id="c526b-116">Int32</span><span class="sxs-lookup"><span data-stu-id="c526b-116">Int32</span></span>|<span data-ttu-id="c526b-117">Tamanho de prefixo.</span><span class="sxs-lookup"><span data-stu-id="c526b-117">Prefix size.</span></span> <span data-ttu-id="c526b-118">(1-32).</span><span class="sxs-lookup"><span data-stu-id="c526b-118">(1-32).</span></span> <span data-ttu-id="c526b-119">Valores válidos 1 a 32</span><span class="sxs-lookup"><span data-stu-id="c526b-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="c526b-120">Relações</span><span class="sxs-lookup"><span data-stu-id="c526b-120">Relationships</span></span>
<span data-ttu-id="c526b-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c526b-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c526b-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c526b-122">JSON Representation</span></span>
<span data-ttu-id="c526b-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c526b-123">Here is a JSON representation of the resource.</span></span>
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




