---
title: tipo de recurso de vpnRoute
description: Definição de rota da VPN.
ms.openlocfilehash: 385ed5f369660805afa8cf935273b6689fc90173
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038444"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="c76a3-103">tipo de recurso de vpnRoute</span><span class="sxs-lookup"><span data-stu-id="c76a3-103">vpnRoute resource type</span></span>

> <span data-ttu-id="c76a3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c76a3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c76a3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c76a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c76a3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c76a3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c76a3-107">Definição de rota da VPN.</span><span class="sxs-lookup"><span data-stu-id="c76a3-107">VPN Route definition.</span></span>
## <a name="properties"></a><span data-ttu-id="c76a3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c76a3-108">Properties</span></span>
|<span data-ttu-id="c76a3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c76a3-109">Property</span></span>|<span data-ttu-id="c76a3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c76a3-110">Type</span></span>|<span data-ttu-id="c76a3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c76a3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c76a3-112">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="c76a3-112">destinationPrefix</span></span>|<span data-ttu-id="c76a3-113">String</span><span class="sxs-lookup"><span data-stu-id="c76a3-113">String</span></span>|<span data-ttu-id="c76a3-114">Prefixo de destino (endereço IPv4/v6).</span><span class="sxs-lookup"><span data-stu-id="c76a3-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="c76a3-115">prefixSize</span><span class="sxs-lookup"><span data-stu-id="c76a3-115">prefixSize</span></span>|<span data-ttu-id="c76a3-116">Int32</span><span class="sxs-lookup"><span data-stu-id="c76a3-116">Int32</span></span>|<span data-ttu-id="c76a3-117">Tamanho de prefixo.</span><span class="sxs-lookup"><span data-stu-id="c76a3-117">Prefix size.</span></span> <span data-ttu-id="c76a3-118">(1-32).</span><span class="sxs-lookup"><span data-stu-id="c76a3-118">(1-32).</span></span> <span data-ttu-id="c76a3-119">Valores válidos 1 a 32</span><span class="sxs-lookup"><span data-stu-id="c76a3-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="c76a3-120">Relações</span><span class="sxs-lookup"><span data-stu-id="c76a3-120">Relationships</span></span>
<span data-ttu-id="c76a3-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c76a3-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c76a3-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c76a3-122">JSON Representation</span></span>
<span data-ttu-id="c76a3-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c76a3-123">Here is a JSON representation of the resource.</span></span>
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





