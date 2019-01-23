---
title: Tipo de recurso windowsInformationProtectionProxiedDomainCollection
description: Coleção de domínios como proxy da Proteção de Informações do Windows
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c65a4b6a94f317c5d75b440aeef7fe387496be32
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421673"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="cec9a-103">Tipo de recurso windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="cec9a-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="cec9a-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="cec9a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cec9a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cec9a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cec9a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="cec9a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cec9a-107">Coleção de domínios como proxy da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="cec9a-107">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="cec9a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cec9a-108">Properties</span></span>
|<span data-ttu-id="cec9a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cec9a-109">Property</span></span>|<span data-ttu-id="cec9a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cec9a-110">Type</span></span>|<span data-ttu-id="cec9a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cec9a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cec9a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="cec9a-112">displayName</span></span>|<span data-ttu-id="cec9a-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cec9a-113">String</span></span>|<span data-ttu-id="cec9a-114">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="cec9a-114">Display name</span></span>|
|<span data-ttu-id="cec9a-115">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="cec9a-115">proxiedDomains</span></span>|<span data-ttu-id="cec9a-116">Coleção [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="cec9a-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="cec9a-117">Coleção de domínios com proxy</span><span class="sxs-lookup"><span data-stu-id="cec9a-117">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="cec9a-118">Relações</span><span class="sxs-lookup"><span data-stu-id="cec9a-118">Relationships</span></span>
<span data-ttu-id="cec9a-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cec9a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cec9a-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cec9a-120">JSON Representation</span></span>
<span data-ttu-id="cec9a-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cec9a-121">Here is a JSON representation of the resource.</span></span>
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




