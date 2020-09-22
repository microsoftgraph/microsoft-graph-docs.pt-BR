---
title: tipo de recurso specifiedCaptiveNetworkPlugins
description: Especifica todos os plugins de rede prisioneiros permitidos durante a conexão VPN AlwaysOn do IKEv2
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 91dde3ebe3508a137d9c01fdd7ee055ba421d6ff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049279"
---
# <a name="specifiedcaptivenetworkplugins-resource-type"></a><span data-ttu-id="1d06c-103">tipo de recurso specifiedCaptiveNetworkPlugins</span><span class="sxs-lookup"><span data-stu-id="1d06c-103">specifiedCaptiveNetworkPlugins resource type</span></span>

<span data-ttu-id="1d06c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d06c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d06c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1d06c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d06c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1d06c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d06c-107">Especifica todos os plugins de rede prisioneiros permitidos durante a conexão VPN AlwaysOn do IKEv2</span><span class="sxs-lookup"><span data-stu-id="1d06c-107">Specifies all the Captive network plugins allowed during the IKEv2 AlwaysOn VPN connection</span></span>

## <a name="properties"></a><span data-ttu-id="1d06c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d06c-108">Properties</span></span>
|<span data-ttu-id="1d06c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d06c-109">Property</span></span>|<span data-ttu-id="1d06c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d06c-110">Type</span></span>|<span data-ttu-id="1d06c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d06c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d06c-112">allowedBundleIdentifiers</span><span class="sxs-lookup"><span data-stu-id="1d06c-112">allowedBundleIdentifiers</span></span>|<span data-ttu-id="1d06c-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d06c-113">String collection</span></span>|<span data-ttu-id="1d06c-114">Endereço do servidor IKEv2.</span><span class="sxs-lookup"><span data-stu-id="1d06c-114">Address of the IKEv2 server.</span></span> <span data-ttu-id="1d06c-115">Deve ser um FQDN, userfqdn, endereço de rede ou ASN1DN</span><span class="sxs-lookup"><span data-stu-id="1d06c-115">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d06c-116">Relações</span><span class="sxs-lookup"><span data-stu-id="1d06c-116">Relationships</span></span>
<span data-ttu-id="1d06c-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1d06c-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d06c-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d06c-118">JSON Representation</span></span>
<span data-ttu-id="1d06c-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d06c-119">Here is a JSON representation of the resource.</span></span>
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






