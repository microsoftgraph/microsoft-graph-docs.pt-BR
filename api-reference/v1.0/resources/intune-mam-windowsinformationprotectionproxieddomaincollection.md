---
title: Tipo de recurso windowsInformationProtectionProxiedDomainCollection
description: Coleção de domínios como proxy da Proteção de Informações do Windows
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 500f662b0a610866ac3e637850f5fd6edeffaa5b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459690"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="7be23-103">Tipo de recurso windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="7be23-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

<span data-ttu-id="7be23-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7be23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7be23-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7be23-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7be23-106">Coleção de domínios como proxy da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="7be23-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="7be23-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7be23-107">Properties</span></span>
|<span data-ttu-id="7be23-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7be23-108">Property</span></span>|<span data-ttu-id="7be23-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7be23-109">Type</span></span>|<span data-ttu-id="7be23-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7be23-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7be23-111">displayName</span><span class="sxs-lookup"><span data-stu-id="7be23-111">displayName</span></span>|<span data-ttu-id="7be23-112">String</span><span class="sxs-lookup"><span data-stu-id="7be23-112">String</span></span>|<span data-ttu-id="7be23-113">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="7be23-113">Display name</span></span>|
|<span data-ttu-id="7be23-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="7be23-114">proxiedDomains</span></span>|<span data-ttu-id="7be23-115">Coleção [proxiedDomain](../resources/intune-mam-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="7be23-115">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="7be23-116">Coleção de domínios com proxy</span><span class="sxs-lookup"><span data-stu-id="7be23-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="7be23-117">Relações</span><span class="sxs-lookup"><span data-stu-id="7be23-117">Relationships</span></span>
<span data-ttu-id="7be23-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7be23-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7be23-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7be23-119">JSON Representation</span></span>
<span data-ttu-id="7be23-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7be23-120">Here is a JSON representation of the resource.</span></span>
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







