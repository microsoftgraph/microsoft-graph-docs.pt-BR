---
title: tipo de recurso specifiedCaptiveNetworkPlugins
description: Especifica todos os plugins de rede prisioneiros permitidos durante a conexão VPN AlwaysOn do IKEv2
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 107c700a35e24cf47b9af2642523ed9b1c735d26
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49276592"
---
# <a name="specifiedcaptivenetworkplugins-resource-type"></a><span data-ttu-id="3a3f5-103">tipo de recurso specifiedCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="3a3f5-103">specifiedCaptiveNetworkPlugins resource type</span></span>

<span data-ttu-id="3a3f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a3f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a3f5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3a3f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a3f5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3a3f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a3f5-107">Especifica todos os plugins de rede prisioneiros permitidos durante a conexão VPN AlwaysOn do IKEv2</span><span class="sxs-lookup"><span data-stu-id="3a3f5-107">Specifies all the Captive network plugins allowed during the IKEv2 AlwaysOn VPN connection</span></span>

## <a name="properties"></a><span data-ttu-id="3a3f5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a3f5-108">Properties</span></span>
|<span data-ttu-id="3a3f5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a3f5-109">Property</span></span>|<span data-ttu-id="3a3f5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a3f5-110">Type</span></span>|<span data-ttu-id="3a3f5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a3f5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a3f5-112">allowedBundleIdentifiers</span><span class="sxs-lookup"><span data-stu-id="3a3f5-112">allowedBundleIdentifiers</span></span>|<span data-ttu-id="3a3f5-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a3f5-113">String collection</span></span>|<span data-ttu-id="3a3f5-114">Endereço do servidor IKEv2.</span><span class="sxs-lookup"><span data-stu-id="3a3f5-114">Address of the IKEv2 server.</span></span> <span data-ttu-id="3a3f5-115">Deve ser um FQDN, userfqdn, endereço de rede ou ASN1DN</span><span class="sxs-lookup"><span data-stu-id="3a3f5-115">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a3f5-116">Relações</span><span class="sxs-lookup"><span data-stu-id="3a3f5-116">Relationships</span></span>
<span data-ttu-id="3a3f5-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3a3f5-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a3f5-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a3f5-118">JSON Representation</span></span>
<span data-ttu-id="3a3f5-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a3f5-119">Here is a JSON representation of the resource.</span></span>
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




