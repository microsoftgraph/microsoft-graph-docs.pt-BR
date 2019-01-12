---
title: tipo de recurso de vpnDnsRule
description: Definição de regra de DNS da VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3c928542f749973ac3abea041c8ca60ee74ff8fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964736"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="a93a3-103">tipo de recurso de vpnDnsRule</span><span class="sxs-lookup"><span data-stu-id="a93a3-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="a93a3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a93a3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a93a3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a93a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a93a3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a93a3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a93a3-107">Definição de regra de DNS da VPN.</span><span class="sxs-lookup"><span data-stu-id="a93a3-107">VPN DNS Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="a93a3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a93a3-108">Properties</span></span>
|<span data-ttu-id="a93a3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a93a3-109">Property</span></span>|<span data-ttu-id="a93a3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a93a3-110">Type</span></span>|<span data-ttu-id="a93a3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a93a3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a93a3-112">name</span><span class="sxs-lookup"><span data-stu-id="a93a3-112">name</span></span>|<span data-ttu-id="a93a3-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a93a3-113">String</span></span>|<span data-ttu-id="a93a3-114">Nome.</span><span class="sxs-lookup"><span data-stu-id="a93a3-114">Name.</span></span>|
|<span data-ttu-id="a93a3-115">servidores</span><span class="sxs-lookup"><span data-stu-id="a93a3-115">servers</span></span>|<span data-ttu-id="a93a3-116">String collection</span><span class="sxs-lookup"><span data-stu-id="a93a3-116">String collection</span></span>|<span data-ttu-id="a93a3-117">Servidores.</span><span class="sxs-lookup"><span data-stu-id="a93a3-117">Servers.</span></span>|
|<span data-ttu-id="a93a3-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="a93a3-118">proxyServerUri</span></span>|<span data-ttu-id="a93a3-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a93a3-119">String</span></span>|<span data-ttu-id="a93a3-120">Uri do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="a93a3-120">Proxy Server Uri.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a93a3-121">Relações</span><span class="sxs-lookup"><span data-stu-id="a93a3-121">Relationships</span></span>
<span data-ttu-id="a93a3-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a93a3-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a93a3-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a93a3-123">JSON Representation</span></span>
<span data-ttu-id="a93a3-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a93a3-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnDnsRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnDnsRule",
  "name": "String",
  "servers": [
    "String"
  ],
  "proxyServerUri": "String"
}
```





