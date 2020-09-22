---
title: Tipo de recurso proxiedDomain
description: Domínio com proxy
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 16995c4ffc959c5a63d322da84bdca136a2422f8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048404"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="99643-103">Tipo de recurso proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="99643-103">proxiedDomain resource type</span></span>

<span data-ttu-id="99643-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99643-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99643-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99643-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99643-106">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="99643-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="99643-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99643-107">Properties</span></span>
|<span data-ttu-id="99643-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99643-108">Property</span></span>|<span data-ttu-id="99643-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="99643-109">Type</span></span>|<span data-ttu-id="99643-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="99643-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99643-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="99643-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="99643-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99643-112">String</span></span>|<span data-ttu-id="99643-113">O endereço IP ou FQDN</span><span class="sxs-lookup"><span data-stu-id="99643-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="99643-114">proxy</span><span class="sxs-lookup"><span data-stu-id="99643-114">proxy</span></span>|<span data-ttu-id="99643-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99643-115">String</span></span>|<span data-ttu-id="99643-116">IP ou FQDN do proxy</span><span class="sxs-lookup"><span data-stu-id="99643-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="99643-117">Relações</span><span class="sxs-lookup"><span data-stu-id="99643-117">Relationships</span></span>
<span data-ttu-id="99643-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99643-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99643-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99643-119">JSON Representation</span></span>
<span data-ttu-id="99643-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99643-120">Here is a JSON representation of the resource.</span></span>
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









