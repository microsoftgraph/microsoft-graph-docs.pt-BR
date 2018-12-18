---
title: Tipo de recurso proxiedDomain
description: Domínio com proxy
author: tfitzmac
ms.openlocfilehash: dc924d75bc2cf1310cb715033281f59b70abb32a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320290"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="8b71c-103">Tipo de recurso proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="8b71c-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="8b71c-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8b71c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b71c-105">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="8b71c-105">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="8b71c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8b71c-106">Properties</span></span>
|<span data-ttu-id="8b71c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b71c-107">Property</span></span>|<span data-ttu-id="8b71c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b71c-108">Type</span></span>|<span data-ttu-id="8b71c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b71c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b71c-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="8b71c-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="8b71c-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b71c-111">String</span></span>|<span data-ttu-id="8b71c-112">O endereço IP ou FQDN</span><span class="sxs-lookup"><span data-stu-id="8b71c-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="8b71c-113">proxy</span><span class="sxs-lookup"><span data-stu-id="8b71c-113">proxy</span></span>|<span data-ttu-id="8b71c-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b71c-114">String</span></span>|<span data-ttu-id="8b71c-115">IP de proxy</span><span class="sxs-lookup"><span data-stu-id="8b71c-115">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b71c-116">Relações</span><span class="sxs-lookup"><span data-stu-id="8b71c-116">Relationships</span></span>
<span data-ttu-id="8b71c-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8b71c-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8b71c-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8b71c-118">JSON Representation</span></span>
<span data-ttu-id="8b71c-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8b71c-119">Here is a JSON representation of the resource.</span></span>
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



