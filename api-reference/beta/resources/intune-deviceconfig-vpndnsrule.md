---
title: tipo de recurso de vpnDnsRule
description: Definição de regra de DNS da VPN.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d09e26b105a139f04db34ba69184fcf60e9ef238
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868198"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="8b1dd-103">tipo de recurso de vpnDnsRule</span><span class="sxs-lookup"><span data-stu-id="8b1dd-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="8b1dd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8b1dd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b1dd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8b1dd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8b1dd-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8b1dd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b1dd-107">Definição de regra de DNS da VPN.</span><span class="sxs-lookup"><span data-stu-id="8b1dd-107">VPN DNS Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="8b1dd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8b1dd-108">Properties</span></span>
|<span data-ttu-id="8b1dd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b1dd-109">Property</span></span>|<span data-ttu-id="8b1dd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b1dd-110">Type</span></span>|<span data-ttu-id="8b1dd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b1dd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b1dd-112">name</span><span class="sxs-lookup"><span data-stu-id="8b1dd-112">name</span></span>|<span data-ttu-id="8b1dd-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b1dd-113">String</span></span>|<span data-ttu-id="8b1dd-114">Nome.</span><span class="sxs-lookup"><span data-stu-id="8b1dd-114">Name.</span></span>|
|<span data-ttu-id="8b1dd-115">servidores</span><span class="sxs-lookup"><span data-stu-id="8b1dd-115">servers</span></span>|<span data-ttu-id="8b1dd-116">String collection</span><span class="sxs-lookup"><span data-stu-id="8b1dd-116">String collection</span></span>|<span data-ttu-id="8b1dd-117">Servidores.</span><span class="sxs-lookup"><span data-stu-id="8b1dd-117">Servers.</span></span>|
|<span data-ttu-id="8b1dd-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="8b1dd-118">proxyServerUri</span></span>|<span data-ttu-id="8b1dd-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b1dd-119">String</span></span>|<span data-ttu-id="8b1dd-120">Uri do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="8b1dd-120">Proxy Server Uri.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b1dd-121">Relações</span><span class="sxs-lookup"><span data-stu-id="8b1dd-121">Relationships</span></span>
<span data-ttu-id="8b1dd-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8b1dd-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8b1dd-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8b1dd-123">JSON Representation</span></span>
<span data-ttu-id="8b1dd-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8b1dd-124">Here is a JSON representation of the resource.</span></span>
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





