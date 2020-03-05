---
title: Tipo de recurso windowsInformationProtectionProxiedDomainCollection
description: Coleção de domínios como proxy da Proteção de Informações do Windows
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5a741f0da4a2219e04c7f3cde43bfb9e7ab9cb63
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527823"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="f314d-103">Tipo de recurso windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="f314d-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

<span data-ttu-id="f314d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f314d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f314d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f314d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f314d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f314d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f314d-107">Coleção de domínios como proxy da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="f314d-107">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="f314d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f314d-108">Properties</span></span>
|<span data-ttu-id="f314d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f314d-109">Property</span></span>|<span data-ttu-id="f314d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f314d-110">Type</span></span>|<span data-ttu-id="f314d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f314d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f314d-112">displayName</span><span class="sxs-lookup"><span data-stu-id="f314d-112">displayName</span></span>|<span data-ttu-id="f314d-113">String</span><span class="sxs-lookup"><span data-stu-id="f314d-113">String</span></span>|<span data-ttu-id="f314d-114">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="f314d-114">Display name</span></span>|
|<span data-ttu-id="f314d-115">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="f314d-115">proxiedDomains</span></span>|<span data-ttu-id="f314d-116">Coleção [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="f314d-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="f314d-117">Coleção de domínios com proxy</span><span class="sxs-lookup"><span data-stu-id="f314d-117">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="f314d-118">Relações</span><span class="sxs-lookup"><span data-stu-id="f314d-118">Relationships</span></span>
<span data-ttu-id="f314d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f314d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f314d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f314d-120">JSON Representation</span></span>
<span data-ttu-id="f314d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f314d-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
  "displayName": "String",
  "proxiedDomains": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ]
}
```



