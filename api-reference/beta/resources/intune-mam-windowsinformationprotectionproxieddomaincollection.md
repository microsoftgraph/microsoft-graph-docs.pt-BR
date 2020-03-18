---
title: Tipo de recurso windowsInformationProtectionProxiedDomainCollection
description: Coleção de domínios como proxy da Proteção de Informações do Windows
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 35c4f00965aa6878368e922a0c193484c90c6aed
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42780357"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="ae1a8-103">Tipo de recurso windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="ae1a8-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="ae1a8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae1a8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae1a8-106">Coleção de domínios como proxy da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="ae1a8-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="ae1a8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae1a8-107">Properties</span></span>
|<span data-ttu-id="ae1a8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae1a8-108">Property</span></span>|<span data-ttu-id="ae1a8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae1a8-109">Type</span></span>|<span data-ttu-id="ae1a8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae1a8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae1a8-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ae1a8-111">displayName</span></span>|<span data-ttu-id="ae1a8-112">String</span><span class="sxs-lookup"><span data-stu-id="ae1a8-112">String</span></span>|<span data-ttu-id="ae1a8-113">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="ae1a8-113">Display name</span></span>|
|<span data-ttu-id="ae1a8-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="ae1a8-114">proxiedDomains</span></span>|<span data-ttu-id="ae1a8-115">Coleção [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="ae1a8-115">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="ae1a8-116">Coleção de domínios com proxy</span><span class="sxs-lookup"><span data-stu-id="ae1a8-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae1a8-117">Relações</span><span class="sxs-lookup"><span data-stu-id="ae1a8-117">Relationships</span></span>
<span data-ttu-id="ae1a8-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ae1a8-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae1a8-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae1a8-119">JSON Representation</span></span>
<span data-ttu-id="ae1a8-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ae1a8-120">Here is a JSON representation of the resource.</span></span>
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



