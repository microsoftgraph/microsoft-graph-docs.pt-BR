---
title: tipo de recurso iosVpnSecurityAssociationParameters
description: Parâmetros de associação de segurança VPN
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d3da905a68222b60bef7225f34afc2b4a0b39a50
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790493"
---
# <a name="iosvpnsecurityassociationparameters-resource-type"></a><span data-ttu-id="8ec6a-103">tipo de recurso iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="8ec6a-103">iosVpnSecurityAssociationParameters resource type</span></span>

> <span data-ttu-id="8ec6a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8ec6a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ec6a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8ec6a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ec6a-106">Parâmetros de associação de segurança VPN</span><span class="sxs-lookup"><span data-stu-id="8ec6a-106">VPN Security Association Parameters</span></span>

## <a name="properties"></a><span data-ttu-id="8ec6a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ec6a-107">Properties</span></span>
|<span data-ttu-id="8ec6a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ec6a-108">Property</span></span>|<span data-ttu-id="8ec6a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ec6a-109">Type</span></span>|<span data-ttu-id="8ec6a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ec6a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ec6a-111">securityEncryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="8ec6a-111">securityEncryptionAlgorithm</span></span>|[<span data-ttu-id="8ec6a-112">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="8ec6a-112">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="8ec6a-113">Algoritmo de criptografia.</span><span class="sxs-lookup"><span data-stu-id="8ec6a-113">Encryption algorithm.</span></span> <span data-ttu-id="8ec6a-114">Os possíveis valores são: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`.</span><span class="sxs-lookup"><span data-stu-id="8ec6a-114">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`.</span></span>|
|<span data-ttu-id="8ec6a-115">securityIntegrityAlgorithm</span><span class="sxs-lookup"><span data-stu-id="8ec6a-115">securityIntegrityAlgorithm</span></span>|[<span data-ttu-id="8ec6a-116">vpnIntegrityAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="8ec6a-116">vpnIntegrityAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|<span data-ttu-id="8ec6a-117">Algoritmo de integridade.</span><span class="sxs-lookup"><span data-stu-id="8ec6a-117">Integrity algorithm.</span></span> <span data-ttu-id="8ec6a-118">Os valores possíveis são: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`.</span><span class="sxs-lookup"><span data-stu-id="8ec6a-118">Possible values are: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`.</span></span>|
|<span data-ttu-id="8ec6a-119">securityDiffieHellmanGroup</span><span class="sxs-lookup"><span data-stu-id="8ec6a-119">securityDiffieHellmanGroup</span></span>|<span data-ttu-id="8ec6a-120">Int32</span><span class="sxs-lookup"><span data-stu-id="8ec6a-120">Int32</span></span>|<span data-ttu-id="8ec6a-121">Grupo Diffie-Hellman</span><span class="sxs-lookup"><span data-stu-id="8ec6a-121">Diffie-Hellman Group</span></span>|
|<span data-ttu-id="8ec6a-122">lifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="8ec6a-122">lifetimeInMinutes</span></span>|<span data-ttu-id="8ec6a-123">Int32</span><span class="sxs-lookup"><span data-stu-id="8ec6a-123">Int32</span></span>|<span data-ttu-id="8ec6a-124">Tempo de vida (minutos)</span><span class="sxs-lookup"><span data-stu-id="8ec6a-124">Lifetime (minutes)</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ec6a-125">Relações</span><span class="sxs-lookup"><span data-stu-id="8ec6a-125">Relationships</span></span>
<span data-ttu-id="8ec6a-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8ec6a-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ec6a-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ec6a-127">JSON Representation</span></span>
<span data-ttu-id="8ec6a-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ec6a-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVpnSecurityAssociationParameters",
  "securityEncryptionAlgorithm": "String",
  "securityIntegrityAlgorithm": "String",
  "securityDiffieHellmanGroup": 1024,
  "lifetimeInMinutes": 1024
}
```



