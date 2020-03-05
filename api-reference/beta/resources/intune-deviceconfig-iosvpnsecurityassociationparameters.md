---
title: tipo de recurso iosVpnSecurityAssociationParameters
description: Parâmetros de associação de segurança VPN
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cd53bec653f072dd22554be4e4255997657ab833
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526280"
---
# <a name="iosvpnsecurityassociationparameters-resource-type"></a><span data-ttu-id="207d0-103">tipo de recurso iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="207d0-103">iosVpnSecurityAssociationParameters resource type</span></span>

<span data-ttu-id="207d0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="207d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="207d0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="207d0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="207d0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="207d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="207d0-107">Parâmetros de associação de segurança VPN</span><span class="sxs-lookup"><span data-stu-id="207d0-107">VPN Security Association Parameters</span></span>

## <a name="properties"></a><span data-ttu-id="207d0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="207d0-108">Properties</span></span>
|<span data-ttu-id="207d0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="207d0-109">Property</span></span>|<span data-ttu-id="207d0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="207d0-110">Type</span></span>|<span data-ttu-id="207d0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="207d0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="207d0-112">securityEncryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="207d0-112">securityEncryptionAlgorithm</span></span>|[<span data-ttu-id="207d0-113">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="207d0-113">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="207d0-114">Algoritmo de criptografia.</span><span class="sxs-lookup"><span data-stu-id="207d0-114">Encryption algorithm.</span></span> <span data-ttu-id="207d0-115">Os possíveis valores são: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`.</span><span class="sxs-lookup"><span data-stu-id="207d0-115">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`.</span></span>|
|<span data-ttu-id="207d0-116">securityIntegrityAlgorithm</span><span class="sxs-lookup"><span data-stu-id="207d0-116">securityIntegrityAlgorithm</span></span>|[<span data-ttu-id="207d0-117">vpnIntegrityAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="207d0-117">vpnIntegrityAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|<span data-ttu-id="207d0-118">Algoritmo de integridade.</span><span class="sxs-lookup"><span data-stu-id="207d0-118">Integrity algorithm.</span></span> <span data-ttu-id="207d0-119">Os valores possíveis são: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`.</span><span class="sxs-lookup"><span data-stu-id="207d0-119">Possible values are: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`.</span></span>|
|<span data-ttu-id="207d0-120">securityDiffieHellmanGroup</span><span class="sxs-lookup"><span data-stu-id="207d0-120">securityDiffieHellmanGroup</span></span>|<span data-ttu-id="207d0-121">Int32</span><span class="sxs-lookup"><span data-stu-id="207d0-121">Int32</span></span>|<span data-ttu-id="207d0-122">Grupo Diffie-Hellman</span><span class="sxs-lookup"><span data-stu-id="207d0-122">Diffie-Hellman Group</span></span>|
|<span data-ttu-id="207d0-123">lifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="207d0-123">lifetimeInMinutes</span></span>|<span data-ttu-id="207d0-124">Int32</span><span class="sxs-lookup"><span data-stu-id="207d0-124">Int32</span></span>|<span data-ttu-id="207d0-125">Tempo de vida (minutos)</span><span class="sxs-lookup"><span data-stu-id="207d0-125">Lifetime (minutes)</span></span>|

## <a name="relationships"></a><span data-ttu-id="207d0-126">Relações</span><span class="sxs-lookup"><span data-stu-id="207d0-126">Relationships</span></span>
<span data-ttu-id="207d0-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="207d0-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="207d0-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="207d0-128">JSON Representation</span></span>
<span data-ttu-id="207d0-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="207d0-129">Here is a JSON representation of the resource.</span></span>
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



