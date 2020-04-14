---
title: Tipo de recurso windowsInformationProtectionProxiedDomainCollection
description: Coleção de domínios como proxy da Proteção de Informações do Windows
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a00cfc03ff6b98bb32b7c8fe7e9d747f15040d68
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43419289"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="48690-103">Tipo de recurso windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="48690-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

<span data-ttu-id="48690-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48690-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="48690-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="48690-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48690-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="48690-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48690-107">Coleção de domínios como proxy da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="48690-107">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="48690-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48690-108">Properties</span></span>
|<span data-ttu-id="48690-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48690-109">Property</span></span>|<span data-ttu-id="48690-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="48690-110">Type</span></span>|<span data-ttu-id="48690-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="48690-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48690-112">displayName</span><span class="sxs-lookup"><span data-stu-id="48690-112">displayName</span></span>|<span data-ttu-id="48690-113">String</span><span class="sxs-lookup"><span data-stu-id="48690-113">String</span></span>|<span data-ttu-id="48690-114">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="48690-114">Display name</span></span>|
|<span data-ttu-id="48690-115">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="48690-115">proxiedDomains</span></span>|<span data-ttu-id="48690-116">Coleção [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="48690-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="48690-117">Coleção de domínios com proxy</span><span class="sxs-lookup"><span data-stu-id="48690-117">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="48690-118">Relações</span><span class="sxs-lookup"><span data-stu-id="48690-118">Relationships</span></span>
<span data-ttu-id="48690-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="48690-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="48690-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48690-120">JSON Representation</span></span>
<span data-ttu-id="48690-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48690-121">Here is a JSON representation of the resource.</span></span>
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



