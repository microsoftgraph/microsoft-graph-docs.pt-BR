---
title: Tipo de recurso windowsInformationProtectionProxiedDomainCollection
description: Coleção de domínios como proxy da Proteção de Informações do Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 987ae09f46c9bb2f0c6dc5481320d07ae250b01c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755725"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="48fff-103">Tipo de recurso windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="48fff-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

<span data-ttu-id="48fff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48fff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="48fff-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="48fff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48fff-106">Coleção de domínios como proxy da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="48fff-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="48fff-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48fff-107">Properties</span></span>
|<span data-ttu-id="48fff-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48fff-108">Property</span></span>|<span data-ttu-id="48fff-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="48fff-109">Type</span></span>|<span data-ttu-id="48fff-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="48fff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48fff-111">displayName</span><span class="sxs-lookup"><span data-stu-id="48fff-111">displayName</span></span>|<span data-ttu-id="48fff-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48fff-112">String</span></span>|<span data-ttu-id="48fff-113">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="48fff-113">Display name</span></span>|
|<span data-ttu-id="48fff-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="48fff-114">proxiedDomains</span></span>|<span data-ttu-id="48fff-115">Coleção [proxiedDomain](../resources/intune-mam-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="48fff-115">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="48fff-116">Coleção de domínios com proxy</span><span class="sxs-lookup"><span data-stu-id="48fff-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="48fff-117">Relações</span><span class="sxs-lookup"><span data-stu-id="48fff-117">Relationships</span></span>
<span data-ttu-id="48fff-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="48fff-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="48fff-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48fff-119">JSON Representation</span></span>
<span data-ttu-id="48fff-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48fff-120">Here is a JSON representation of the resource.</span></span>
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




