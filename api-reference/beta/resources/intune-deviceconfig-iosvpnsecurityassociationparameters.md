---
title: tipo de recurso iosVpnSecurityAssociationParameters
description: Parâmetros de associação de segurança VPN
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c751c799c385c09d60aa7c57db8425173d093151
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702527"
---
# <a name="iosvpnsecurityassociationparameters-resource-type"></a><span data-ttu-id="7c9a3-103">tipo de recurso iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="7c9a3-103">iosVpnSecurityAssociationParameters resource type</span></span>

<span data-ttu-id="7c9a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c9a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c9a3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7c9a3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c9a3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c9a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c9a3-107">Parâmetros de associação de segurança VPN</span><span class="sxs-lookup"><span data-stu-id="7c9a3-107">VPN Security Association Parameters</span></span>

## <a name="properties"></a><span data-ttu-id="7c9a3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7c9a3-108">Properties</span></span>
|<span data-ttu-id="7c9a3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c9a3-109">Property</span></span>|<span data-ttu-id="7c9a3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c9a3-110">Type</span></span>|<span data-ttu-id="7c9a3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c9a3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c9a3-112">securityEncryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="7c9a3-112">securityEncryptionAlgorithm</span></span>|[<span data-ttu-id="7c9a3-113">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="7c9a3-113">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="7c9a3-114">Algoritmo de criptografia.</span><span class="sxs-lookup"><span data-stu-id="7c9a3-114">Encryption algorithm.</span></span> <span data-ttu-id="7c9a3-115">Os valores possíveis são: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span><span class="sxs-lookup"><span data-stu-id="7c9a3-115">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span></span>|
|<span data-ttu-id="7c9a3-116">securityIntegrityAlgorithm</span><span class="sxs-lookup"><span data-stu-id="7c9a3-116">securityIntegrityAlgorithm</span></span>|[<span data-ttu-id="7c9a3-117">vpnIntegrityAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="7c9a3-117">vpnIntegrityAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|<span data-ttu-id="7c9a3-118">Algoritmo de integridade.</span><span class="sxs-lookup"><span data-stu-id="7c9a3-118">Integrity algorithm.</span></span> <span data-ttu-id="7c9a3-119">Os possíveis valores são: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.</span><span class="sxs-lookup"><span data-stu-id="7c9a3-119">Possible values are: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.</span></span>|
|<span data-ttu-id="7c9a3-120">securityDiffieHellmanGroup</span><span class="sxs-lookup"><span data-stu-id="7c9a3-120">securityDiffieHellmanGroup</span></span>|<span data-ttu-id="7c9a3-121">Int32</span><span class="sxs-lookup"><span data-stu-id="7c9a3-121">Int32</span></span>|<span data-ttu-id="7c9a3-122">Diffie-Hellman grupo</span><span class="sxs-lookup"><span data-stu-id="7c9a3-122">Diffie-Hellman Group</span></span>|
|<span data-ttu-id="7c9a3-123">lifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="7c9a3-123">lifetimeInMinutes</span></span>|<span data-ttu-id="7c9a3-124">Int32</span><span class="sxs-lookup"><span data-stu-id="7c9a3-124">Int32</span></span>|<span data-ttu-id="7c9a3-125">Tempo de vida (minutos)</span><span class="sxs-lookup"><span data-stu-id="7c9a3-125">Lifetime (minutes)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c9a3-126">Relações</span><span class="sxs-lookup"><span data-stu-id="7c9a3-126">Relationships</span></span>
<span data-ttu-id="7c9a3-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7c9a3-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c9a3-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7c9a3-128">JSON Representation</span></span>
<span data-ttu-id="7c9a3-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7c9a3-129">Here is a JSON representation of the resource.</span></span>
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





