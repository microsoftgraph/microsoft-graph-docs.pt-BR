---
title: tipo de recurso cryptographySuite
description: Parâmetros de associação de segurança VPN
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9e2de92f47203888df2e167ae06e025b1cad0190
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729802"
---
# <a name="cryptographysuite-resource-type"></a><span data-ttu-id="2cd43-103">tipo de recurso cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="2cd43-103">cryptographySuite resource type</span></span>

<span data-ttu-id="2cd43-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cd43-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2cd43-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2cd43-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cd43-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2cd43-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cd43-107">Parâmetros de associação de segurança VPN</span><span class="sxs-lookup"><span data-stu-id="2cd43-107">VPN Security Association Parameters</span></span>

## <a name="properties"></a><span data-ttu-id="2cd43-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2cd43-108">Properties</span></span>
|<span data-ttu-id="2cd43-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2cd43-109">Property</span></span>|<span data-ttu-id="2cd43-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2cd43-110">Type</span></span>|<span data-ttu-id="2cd43-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cd43-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cd43-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="2cd43-112">encryptionMethod</span></span>|[<span data-ttu-id="2cd43-113">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="2cd43-113">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="2cd43-114">Método de criptografia.</span><span class="sxs-lookup"><span data-stu-id="2cd43-114">Encryption Method.</span></span> <span data-ttu-id="2cd43-115">Os valores possíveis são: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span><span class="sxs-lookup"><span data-stu-id="2cd43-115">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span></span>|
|<span data-ttu-id="2cd43-116">integrityCheckMethod</span><span class="sxs-lookup"><span data-stu-id="2cd43-116">integrityCheckMethod</span></span>|[<span data-ttu-id="2cd43-117">vpnIntegrityAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="2cd43-117">vpnIntegrityAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|<span data-ttu-id="2cd43-118">Método de verificação de integridade.</span><span class="sxs-lookup"><span data-stu-id="2cd43-118">Integrity Check Method.</span></span> <span data-ttu-id="2cd43-119">Os possíveis valores são: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.</span><span class="sxs-lookup"><span data-stu-id="2cd43-119">Possible values are: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.</span></span>|
|<span data-ttu-id="2cd43-120">dhGroup</span><span class="sxs-lookup"><span data-stu-id="2cd43-120">dhGroup</span></span>|[<span data-ttu-id="2cd43-121">diffieHellmanGroup</span><span class="sxs-lookup"><span data-stu-id="2cd43-121">diffieHellmanGroup</span></span>](../resources/intune-deviceconfig-diffiehellmangroup.md)|<span data-ttu-id="2cd43-122">Grupo Diffie Hellman.</span><span class="sxs-lookup"><span data-stu-id="2cd43-122">Diffie Hellman Group.</span></span> <span data-ttu-id="2cd43-123">Os possíveis valores são: `group1`, `group2`, `group14`, `ecp256`, `ecp384`, `group24`.</span><span class="sxs-lookup"><span data-stu-id="2cd43-123">Possible values are: `group1`, `group2`, `group14`, `ecp256`, `ecp384`, `group24`.</span></span>|
|<span data-ttu-id="2cd43-124">cipherTransformConstants</span><span class="sxs-lookup"><span data-stu-id="2cd43-124">cipherTransformConstants</span></span>|[<span data-ttu-id="2cd43-125">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="2cd43-125">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="2cd43-126">Constantes de transformação de codificação.</span><span class="sxs-lookup"><span data-stu-id="2cd43-126">Cipher Transform Constants.</span></span> <span data-ttu-id="2cd43-127">Os valores possíveis são: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span><span class="sxs-lookup"><span data-stu-id="2cd43-127">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span></span>|
|<span data-ttu-id="2cd43-128">authenticationTransformConstants</span><span class="sxs-lookup"><span data-stu-id="2cd43-128">authenticationTransformConstants</span></span>|[<span data-ttu-id="2cd43-129">authenticationTransformConstant</span><span class="sxs-lookup"><span data-stu-id="2cd43-129">authenticationTransformConstant</span></span>](../resources/intune-deviceconfig-authenticationtransformconstant.md)|<span data-ttu-id="2cd43-130">Constantes de transformação de autenticação.</span><span class="sxs-lookup"><span data-stu-id="2cd43-130">Authentication Transform Constants.</span></span> <span data-ttu-id="2cd43-131">Os possíveis valores são: `md5_96`, `sha1_96`, `sha_256_128`, `aes128Gcm`, `aes192Gcm`, `aes256Gcm`.</span><span class="sxs-lookup"><span data-stu-id="2cd43-131">Possible values are: `md5_96`, `sha1_96`, `sha_256_128`, `aes128Gcm`, `aes192Gcm`, `aes256Gcm`.</span></span>|
|<span data-ttu-id="2cd43-132">pfsGroup</span><span class="sxs-lookup"><span data-stu-id="2cd43-132">pfsGroup</span></span>|[<span data-ttu-id="2cd43-133">perfectForwardSecrecyGroup</span><span class="sxs-lookup"><span data-stu-id="2cd43-133">perfectForwardSecrecyGroup</span></span>](../resources/intune-deviceconfig-perfectforwardsecrecygroup.md)|<span data-ttu-id="2cd43-134">Grupo de sigilo total no futuro.</span><span class="sxs-lookup"><span data-stu-id="2cd43-134">Perfect Forward Secrecy Group.</span></span> <span data-ttu-id="2cd43-135">Os valores possíveis são: `pfs1`, `pfs2`, `pfs2048`, `ecp256`, `ecp384`, `pfsMM`, `pfs24`.</span><span class="sxs-lookup"><span data-stu-id="2cd43-135">Possible values are: `pfs1`, `pfs2`, `pfs2048`, `ecp256`, `ecp384`, `pfsMM`, `pfs24`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cd43-136">Relações</span><span class="sxs-lookup"><span data-stu-id="2cd43-136">Relationships</span></span>
<span data-ttu-id="2cd43-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2cd43-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2cd43-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2cd43-138">JSON Representation</span></span>
<span data-ttu-id="2cd43-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2cd43-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cryptographySuite"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cryptographySuite",
  "encryptionMethod": "String",
  "integrityCheckMethod": "String",
  "dhGroup": "String",
  "cipherTransformConstants": "String",
  "authenticationTransformConstants": "String",
  "pfsGroup": "String"
}
```





