---
title: tipo de recurso specifiedCaptiveNetworkPlugins
description: Especifica todos os plugins de rede prisioneiros permitidos durante a conexão VPN AlwaysOn do IKEv2
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 30acdd502e13d2cf4ad1e5167978d1e675e2664a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787485"
---
# <a name="specifiedcaptivenetworkplugins-resource-type"></a><span data-ttu-id="c7688-103">tipo de recurso specifiedCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="c7688-103">specifiedCaptiveNetworkPlugins resource type</span></span>

> <span data-ttu-id="c7688-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7688-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7688-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7688-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7688-106">Especifica todos os plugins de rede prisioneiros permitidos durante a conexão VPN AlwaysOn do IKEv2</span><span class="sxs-lookup"><span data-stu-id="c7688-106">Specifies all the Captive network plugins allowed during the IKEv2 AlwaysOn VPN connection</span></span>

## <a name="properties"></a><span data-ttu-id="c7688-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7688-107">Properties</span></span>
|<span data-ttu-id="c7688-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7688-108">Property</span></span>|<span data-ttu-id="c7688-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7688-109">Type</span></span>|<span data-ttu-id="c7688-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7688-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7688-111">allowedBundleIdentifiers</span><span class="sxs-lookup"><span data-stu-id="c7688-111">allowedBundleIdentifiers</span></span>|<span data-ttu-id="c7688-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7688-112">String collection</span></span>|<span data-ttu-id="c7688-113">Endereço do servidor IKEv2.</span><span class="sxs-lookup"><span data-stu-id="c7688-113">Address of the IKEv2 server.</span></span> <span data-ttu-id="c7688-114">Deve ser um FQDN, userfqdn, endereço de rede ou ASN1DN</span><span class="sxs-lookup"><span data-stu-id="c7688-114">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7688-115">Relações</span><span class="sxs-lookup"><span data-stu-id="c7688-115">Relationships</span></span>
<span data-ttu-id="c7688-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c7688-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7688-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7688-117">JSON Representation</span></span>
<span data-ttu-id="c7688-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7688-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.specifiedCaptiveNetworkPlugins",
  "allowedBundleIdentifiers": [
    "String"
  ]
}
```



