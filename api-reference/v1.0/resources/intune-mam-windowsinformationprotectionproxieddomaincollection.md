---
title: Tipo de recurso windowsInformationProtectionProxiedDomainCollection
description: Coleção de domínios como proxy da Proteção de Informações do Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8df7439bec871e8b4c7ea1a8f15829b60f2fa21f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086526"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="f3967-103">Tipo de recurso windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="f3967-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

<span data-ttu-id="f3967-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3967-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3967-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3967-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3967-106">Coleção de domínios como proxy da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="f3967-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="f3967-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3967-107">Properties</span></span>
|<span data-ttu-id="f3967-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3967-108">Property</span></span>|<span data-ttu-id="f3967-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3967-109">Type</span></span>|<span data-ttu-id="f3967-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3967-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3967-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f3967-111">displayName</span></span>|<span data-ttu-id="f3967-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3967-112">String</span></span>|<span data-ttu-id="f3967-113">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="f3967-113">Display name</span></span>|
|<span data-ttu-id="f3967-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="f3967-114">proxiedDomains</span></span>|<span data-ttu-id="f3967-115">Coleção [proxiedDomain](../resources/intune-mam-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="f3967-115">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="f3967-116">Coleção de domínios com proxy</span><span class="sxs-lookup"><span data-stu-id="f3967-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3967-117">Relações</span><span class="sxs-lookup"><span data-stu-id="f3967-117">Relationships</span></span>
<span data-ttu-id="f3967-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f3967-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3967-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3967-119">JSON Representation</span></span>
<span data-ttu-id="f3967-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f3967-120">Here is a JSON representation of the resource.</span></span>
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









