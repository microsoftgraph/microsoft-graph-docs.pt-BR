---
title: Tipo de recurso windowsInformationProtectionProxiedDomainCollection
description: Coleção de domínios como proxy da Proteção de Informações do Windows
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 11aa9af0dc075e7c07c61923722810e131bf2250
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448204"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="04a37-103">Tipo de recurso windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="04a37-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

<span data-ttu-id="04a37-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="04a37-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04a37-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04a37-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04a37-106">Coleção de domínios como proxy da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="04a37-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="04a37-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04a37-107">Properties</span></span>
|<span data-ttu-id="04a37-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04a37-108">Property</span></span>|<span data-ttu-id="04a37-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="04a37-109">Type</span></span>|<span data-ttu-id="04a37-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="04a37-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04a37-111">displayName</span><span class="sxs-lookup"><span data-stu-id="04a37-111">displayName</span></span>|<span data-ttu-id="04a37-112">String</span><span class="sxs-lookup"><span data-stu-id="04a37-112">String</span></span>|<span data-ttu-id="04a37-113">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="04a37-113">Display name</span></span>|
|<span data-ttu-id="04a37-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="04a37-114">proxiedDomains</span></span>|<span data-ttu-id="04a37-115">Coleção [proxiedDomain](../resources/intune-mam-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="04a37-115">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="04a37-116">Coleção de domínios com proxy</span><span class="sxs-lookup"><span data-stu-id="04a37-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="04a37-117">Relações</span><span class="sxs-lookup"><span data-stu-id="04a37-117">Relationships</span></span>
<span data-ttu-id="04a37-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04a37-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04a37-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04a37-119">JSON Representation</span></span>
<span data-ttu-id="04a37-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04a37-120">Here is a JSON representation of the resource.</span></span>
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




