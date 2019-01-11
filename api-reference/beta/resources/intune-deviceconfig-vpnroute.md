---
title: tipo de recurso de vpnRoute
description: Definição de rota da VPN.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: eaa74a1cef7d2eee8148e240cd80ca72f94adcb4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860568"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="ee203-103">tipo de recurso de vpnRoute</span><span class="sxs-lookup"><span data-stu-id="ee203-103">vpnRoute resource type</span></span>

> <span data-ttu-id="ee203-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ee203-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee203-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ee203-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee203-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ee203-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee203-107">Definição de rota da VPN.</span><span class="sxs-lookup"><span data-stu-id="ee203-107">VPN Route definition.</span></span>
## <a name="properties"></a><span data-ttu-id="ee203-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee203-108">Properties</span></span>
|<span data-ttu-id="ee203-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee203-109">Property</span></span>|<span data-ttu-id="ee203-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee203-110">Type</span></span>|<span data-ttu-id="ee203-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee203-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee203-112">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="ee203-112">destinationPrefix</span></span>|<span data-ttu-id="ee203-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee203-113">String</span></span>|<span data-ttu-id="ee203-114">Prefixo de destino (endereço IPv4/v6).</span><span class="sxs-lookup"><span data-stu-id="ee203-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="ee203-115">prefixSize</span><span class="sxs-lookup"><span data-stu-id="ee203-115">prefixSize</span></span>|<span data-ttu-id="ee203-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ee203-116">Int32</span></span>|<span data-ttu-id="ee203-117">Tamanho de prefixo.</span><span class="sxs-lookup"><span data-stu-id="ee203-117">Prefix size.</span></span> <span data-ttu-id="ee203-118">(1-32).</span><span class="sxs-lookup"><span data-stu-id="ee203-118">(1-32).</span></span> <span data-ttu-id="ee203-119">Valores válidos 1 a 32</span><span class="sxs-lookup"><span data-stu-id="ee203-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee203-120">Relações</span><span class="sxs-lookup"><span data-stu-id="ee203-120">Relationships</span></span>
<span data-ttu-id="ee203-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee203-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ee203-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee203-122">JSON Representation</span></span>
<span data-ttu-id="ee203-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee203-123">Here is a JSON representation of the resource.</span></span>
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





