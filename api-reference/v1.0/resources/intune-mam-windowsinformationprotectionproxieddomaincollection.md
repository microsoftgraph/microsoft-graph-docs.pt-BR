---
title: Tipo de recurso windowsInformationProtectionProxiedDomainCollection
description: Coleção de domínios como proxy da Proteção de Informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0de9ee342cdb0fb42460d9118c87ed7e2a747b55
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037629"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="9a776-103">Tipo de recurso windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="9a776-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="9a776-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9a776-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a776-105">Coleção de domínios como proxy da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="9a776-105">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="9a776-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a776-106">Properties</span></span>
|<span data-ttu-id="9a776-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a776-107">Property</span></span>|<span data-ttu-id="9a776-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a776-108">Type</span></span>|<span data-ttu-id="9a776-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a776-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a776-110">displayName</span><span class="sxs-lookup"><span data-stu-id="9a776-110">displayName</span></span>|<span data-ttu-id="9a776-111">String</span><span class="sxs-lookup"><span data-stu-id="9a776-111">String</span></span>|<span data-ttu-id="9a776-112">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="9a776-112">Display name</span></span>|
|<span data-ttu-id="9a776-113">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="9a776-113">proxiedDomains</span></span>|<span data-ttu-id="9a776-114">Coleção [proxiedDomain](../resources/intune-mam-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="9a776-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="9a776-115">Coleção de domínios com proxy</span><span class="sxs-lookup"><span data-stu-id="9a776-115">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a776-116">Relações</span><span class="sxs-lookup"><span data-stu-id="9a776-116">Relationships</span></span>
<span data-ttu-id="9a776-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9a776-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a776-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a776-118">JSON Representation</span></span>
<span data-ttu-id="9a776-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a776-119">Here is a JSON representation of the resource.</span></span>
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



