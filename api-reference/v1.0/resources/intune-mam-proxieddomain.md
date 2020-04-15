---
title: Tipo de recurso proxiedDomain
description: Domínio com proxy
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6079a2503004a1606e9db0e4b20dce8725f37ab9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474100"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="ede36-103">Tipo de recurso proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="ede36-103">proxiedDomain resource type</span></span>

<span data-ttu-id="ede36-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ede36-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ede36-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ede36-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ede36-106">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="ede36-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="ede36-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ede36-107">Properties</span></span>
|<span data-ttu-id="ede36-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ede36-108">Property</span></span>|<span data-ttu-id="ede36-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ede36-109">Type</span></span>|<span data-ttu-id="ede36-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ede36-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ede36-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="ede36-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="ede36-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ede36-112">String</span></span>|<span data-ttu-id="ede36-113">O endereço IP ou FQDN</span><span class="sxs-lookup"><span data-stu-id="ede36-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="ede36-114">proxy</span><span class="sxs-lookup"><span data-stu-id="ede36-114">proxy</span></span>|<span data-ttu-id="ede36-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ede36-115">String</span></span>|<span data-ttu-id="ede36-116">IP ou FQDN do proxy</span><span class="sxs-lookup"><span data-stu-id="ede36-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="ede36-117">Relações</span><span class="sxs-lookup"><span data-stu-id="ede36-117">Relationships</span></span>
<span data-ttu-id="ede36-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ede36-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ede36-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ede36-119">JSON Representation</span></span>
<span data-ttu-id="ede36-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ede36-120">Here is a JSON representation of the resource.</span></span>
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







