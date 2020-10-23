---
title: tipo de recurso specifiedCaptiveNetworkPlugins
description: Especifica todos os plugins de rede prisioneiros permitidos durante a conexão VPN AlwaysOn do IKEv2
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 48eb34968901e388ae90334ed372bd776a48aaff
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693812"
---
# <a name="specifiedcaptivenetworkplugins-resource-type"></a><span data-ttu-id="97ffa-103">tipo de recurso specifiedCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="97ffa-103">specifiedCaptiveNetworkPlugins resource type</span></span>

<span data-ttu-id="97ffa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97ffa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97ffa-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="97ffa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97ffa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="97ffa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97ffa-107">Especifica todos os plugins de rede prisioneiros permitidos durante a conexão VPN AlwaysOn do IKEv2</span><span class="sxs-lookup"><span data-stu-id="97ffa-107">Specifies all the Captive network plugins allowed during the IKEv2 AlwaysOn VPN connection</span></span>

## <a name="properties"></a><span data-ttu-id="97ffa-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="97ffa-108">Properties</span></span>
|<span data-ttu-id="97ffa-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97ffa-109">Property</span></span>|<span data-ttu-id="97ffa-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="97ffa-110">Type</span></span>|<span data-ttu-id="97ffa-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="97ffa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97ffa-112">allowedBundleIdentifiers</span><span class="sxs-lookup"><span data-stu-id="97ffa-112">allowedBundleIdentifiers</span></span>|<span data-ttu-id="97ffa-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="97ffa-113">String collection</span></span>|<span data-ttu-id="97ffa-114">Endereço do servidor IKEv2.</span><span class="sxs-lookup"><span data-stu-id="97ffa-114">Address of the IKEv2 server.</span></span> <span data-ttu-id="97ffa-115">Deve ser um FQDN, userfqdn, endereço de rede ou ASN1DN</span><span class="sxs-lookup"><span data-stu-id="97ffa-115">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|

## <a name="relationships"></a><span data-ttu-id="97ffa-116">Relações</span><span class="sxs-lookup"><span data-stu-id="97ffa-116">Relationships</span></span>
<span data-ttu-id="97ffa-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="97ffa-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97ffa-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97ffa-118">JSON Representation</span></span>
<span data-ttu-id="97ffa-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="97ffa-119">Here is a JSON representation of the resource.</span></span>
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





