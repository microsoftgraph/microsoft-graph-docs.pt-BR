---
title: Tipo de recurso proxiedDomain
description: Domínio com proxy
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: eff345414531b0ddda1600bb567aacd4a5436602
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871110"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="5e2bf-103">Tipo de recurso proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="5e2bf-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="5e2bf-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5e2bf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e2bf-105">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="5e2bf-105">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="5e2bf-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e2bf-106">Properties</span></span>
|<span data-ttu-id="5e2bf-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e2bf-107">Property</span></span>|<span data-ttu-id="5e2bf-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e2bf-108">Type</span></span>|<span data-ttu-id="5e2bf-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e2bf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e2bf-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="5e2bf-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="5e2bf-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e2bf-111">String</span></span>|<span data-ttu-id="5e2bf-112">O endereço IP ou FQDN</span><span class="sxs-lookup"><span data-stu-id="5e2bf-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="5e2bf-113">proxy</span><span class="sxs-lookup"><span data-stu-id="5e2bf-113">proxy</span></span>|<span data-ttu-id="5e2bf-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e2bf-114">String</span></span>|<span data-ttu-id="5e2bf-115">IP de proxy</span><span class="sxs-lookup"><span data-stu-id="5e2bf-115">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e2bf-116">Relações</span><span class="sxs-lookup"><span data-stu-id="5e2bf-116">Relationships</span></span>
<span data-ttu-id="5e2bf-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5e2bf-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5e2bf-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e2bf-118">JSON Representation</span></span>
<span data-ttu-id="5e2bf-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5e2bf-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```



