---
title: Tipo de recurso proxiedDomain
description: Domínio com proxy
ms.openlocfilehash: d73ed20341a7de025f6f2d39536a1e791b978f55
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005975"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="b11d0-103">Tipo de recurso proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="b11d0-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="b11d0-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b11d0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b11d0-105">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="b11d0-105">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="b11d0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b11d0-106">Properties</span></span>
|<span data-ttu-id="b11d0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b11d0-107">Property</span></span>|<span data-ttu-id="b11d0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b11d0-108">Type</span></span>|<span data-ttu-id="b11d0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b11d0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b11d0-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="b11d0-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="b11d0-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b11d0-111">String</span></span>|<span data-ttu-id="b11d0-112">O endereço IP ou FQDN</span><span class="sxs-lookup"><span data-stu-id="b11d0-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="b11d0-113">proxy</span><span class="sxs-lookup"><span data-stu-id="b11d0-113">proxy</span></span>|<span data-ttu-id="b11d0-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b11d0-114">String</span></span>|<span data-ttu-id="b11d0-115">IP de proxy</span><span class="sxs-lookup"><span data-stu-id="b11d0-115">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="b11d0-116">Relações</span><span class="sxs-lookup"><span data-stu-id="b11d0-116">Relationships</span></span>
<span data-ttu-id="b11d0-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b11d0-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b11d0-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b11d0-118">JSON Representation</span></span>
<span data-ttu-id="b11d0-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b11d0-119">Here is a JSON representation of the resource.</span></span>
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



