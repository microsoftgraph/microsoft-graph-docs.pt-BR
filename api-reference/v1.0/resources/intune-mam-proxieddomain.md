---
title: Tipo de recurso proxiedDomain
description: Domínio com proxy
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 25914b3cba48120e91352028bb51bcdee8edee2b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752319"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="259be-103">Tipo de recurso proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="259be-103">proxiedDomain resource type</span></span>

<span data-ttu-id="259be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="259be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="259be-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="259be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="259be-106">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="259be-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="259be-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="259be-107">Properties</span></span>
|<span data-ttu-id="259be-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="259be-108">Property</span></span>|<span data-ttu-id="259be-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="259be-109">Type</span></span>|<span data-ttu-id="259be-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="259be-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="259be-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="259be-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="259be-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="259be-112">String</span></span>|<span data-ttu-id="259be-113">O endereço IP ou FQDN</span><span class="sxs-lookup"><span data-stu-id="259be-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="259be-114">proxy</span><span class="sxs-lookup"><span data-stu-id="259be-114">proxy</span></span>|<span data-ttu-id="259be-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="259be-115">String</span></span>|<span data-ttu-id="259be-116">IP proxy ou FQDN</span><span class="sxs-lookup"><span data-stu-id="259be-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="259be-117">Relações</span><span class="sxs-lookup"><span data-stu-id="259be-117">Relationships</span></span>
<span data-ttu-id="259be-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="259be-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="259be-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="259be-119">JSON Representation</span></span>
<span data-ttu-id="259be-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="259be-120">Here is a JSON representation of the resource.</span></span>
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




