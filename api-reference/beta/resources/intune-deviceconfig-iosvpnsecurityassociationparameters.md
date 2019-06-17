---
title: tipo de recurso iosVpnSecurityAssociationParameters
description: Parâmetros de associação de segurança VPN
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ecf2597222a578d342f69c16c665c493b8c3329
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002725"
---
# <a name="iosvpnsecurityassociationparameters-resource-type"></a><span data-ttu-id="3f9e3-103">tipo de recurso iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="3f9e3-103">iosVpnSecurityAssociationParameters resource type</span></span>

> <span data-ttu-id="3f9e3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3f9e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f9e3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3f9e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f9e3-106">Parâmetros de associação de segurança VPN</span><span class="sxs-lookup"><span data-stu-id="3f9e3-106">VPN Security Association Parameters</span></span>

## <a name="properties"></a><span data-ttu-id="3f9e3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f9e3-107">Properties</span></span>
|<span data-ttu-id="3f9e3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f9e3-108">Property</span></span>|<span data-ttu-id="3f9e3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f9e3-109">Type</span></span>|<span data-ttu-id="3f9e3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f9e3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f9e3-111">securityEncryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="3f9e3-111">securityEncryptionAlgorithm</span></span>|[<span data-ttu-id="3f9e3-112">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="3f9e3-112">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="3f9e3-113">Algoritmo de criptografia.</span><span class="sxs-lookup"><span data-stu-id="3f9e3-113">Encryption algorithm.</span></span> <span data-ttu-id="3f9e3-114">Os possíveis valores são: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`.</span><span class="sxs-lookup"><span data-stu-id="3f9e3-114">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`.</span></span>|
|<span data-ttu-id="3f9e3-115">securityIntegrityAlgorithm</span><span class="sxs-lookup"><span data-stu-id="3f9e3-115">securityIntegrityAlgorithm</span></span>|[<span data-ttu-id="3f9e3-116">vpnIntegrityAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="3f9e3-116">vpnIntegrityAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|<span data-ttu-id="3f9e3-117">Algoritmo de integridade.</span><span class="sxs-lookup"><span data-stu-id="3f9e3-117">Integrity algorithm.</span></span> <span data-ttu-id="3f9e3-118">Os valores possíveis são: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`.</span><span class="sxs-lookup"><span data-stu-id="3f9e3-118">Possible values are: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`.</span></span>|
|<span data-ttu-id="3f9e3-119">securityDiffieHellmanGroup</span><span class="sxs-lookup"><span data-stu-id="3f9e3-119">securityDiffieHellmanGroup</span></span>|<span data-ttu-id="3f9e3-120">Int32</span><span class="sxs-lookup"><span data-stu-id="3f9e3-120">Int32</span></span>|<span data-ttu-id="3f9e3-121">Grupo Diffie-Hellman</span><span class="sxs-lookup"><span data-stu-id="3f9e3-121">Diffie-Hellman Group</span></span>|
|<span data-ttu-id="3f9e3-122">lifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="3f9e3-122">lifetimeInMinutes</span></span>|<span data-ttu-id="3f9e3-123">Int32</span><span class="sxs-lookup"><span data-stu-id="3f9e3-123">Int32</span></span>|<span data-ttu-id="3f9e3-124">Tempo de vida (minutos)</span><span class="sxs-lookup"><span data-stu-id="3f9e3-124">Lifetime (minutes)</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f9e3-125">Relações</span><span class="sxs-lookup"><span data-stu-id="3f9e3-125">Relationships</span></span>
<span data-ttu-id="3f9e3-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3f9e3-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f9e3-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f9e3-127">JSON Representation</span></span>
<span data-ttu-id="3f9e3-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3f9e3-128">Here is a JSON representation of the resource.</span></span>
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





