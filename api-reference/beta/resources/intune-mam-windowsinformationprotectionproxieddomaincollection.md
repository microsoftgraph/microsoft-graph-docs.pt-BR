---
title: Tipo de recurso windowsInformationProtectionProxiedDomainCollection
description: Coleção de domínios como proxy da Proteção de Informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0cf20d0a0afb33732278b9c8f988b3008854b770
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558290"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="c215e-103">Tipo de recurso windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="c215e-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="c215e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c215e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c215e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c215e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c215e-106">Coleção de domínios como proxy da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="c215e-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="c215e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c215e-107">Properties</span></span>
|<span data-ttu-id="c215e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c215e-108">Property</span></span>|<span data-ttu-id="c215e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c215e-109">Type</span></span>|<span data-ttu-id="c215e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c215e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c215e-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c215e-111">displayName</span></span>|<span data-ttu-id="c215e-112">String</span><span class="sxs-lookup"><span data-stu-id="c215e-112">String</span></span>|<span data-ttu-id="c215e-113">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="c215e-113">Display name</span></span>|
|<span data-ttu-id="c215e-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="c215e-114">proxiedDomains</span></span>|<span data-ttu-id="c215e-115">Coleção [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="c215e-115">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="c215e-116">Coleção de domínios com proxy</span><span class="sxs-lookup"><span data-stu-id="c215e-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="c215e-117">Relações</span><span class="sxs-lookup"><span data-stu-id="c215e-117">Relationships</span></span>
<span data-ttu-id="c215e-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c215e-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c215e-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c215e-119">JSON Representation</span></span>
<span data-ttu-id="c215e-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c215e-120">Here is a JSON representation of the resource.</span></span>
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





