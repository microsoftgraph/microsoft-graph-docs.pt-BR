---
title: tipo de recurso bitLockerFixedDrivePolicy
description: Políticas de unidade fixa do BitLocker.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 326d9c873fd1e0b6b00656aa6b831b7e05ac6bf0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947516"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a><span data-ttu-id="37832-103">tipo de recurso bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="37832-103">bitLockerFixedDrivePolicy resource type</span></span>

> <span data-ttu-id="37832-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="37832-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37832-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37832-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37832-106">Políticas de unidade fixa do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="37832-106">BitLocker Fixed Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="37832-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37832-107">Properties</span></span>
|<span data-ttu-id="37832-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37832-108">Property</span></span>|<span data-ttu-id="37832-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="37832-109">Type</span></span>|<span data-ttu-id="37832-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="37832-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37832-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="37832-111">encryptionMethod</span></span>|[<span data-ttu-id="37832-112">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="37832-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="37832-113">Selecione o método de criptografia para unidades fixas.</span><span class="sxs-lookup"><span data-stu-id="37832-113">Select the encryption method for fixed drives.</span></span> <span data-ttu-id="37832-114">Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="37832-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="37832-115">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="37832-115">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="37832-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="37832-116">Boolean</span></span>|<span data-ttu-id="37832-117">Essa configuração de política determina se é necessário proteger o BitLocker para unidades de dados fixas em um computador.</span><span class="sxs-lookup"><span data-stu-id="37832-117">This policy setting determines whether BitLocker protection is required for fixed data drives to be writable on a computer.</span></span>|
|<span data-ttu-id="37832-118">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="37832-118">recoveryOptions</span></span>|[<span data-ttu-id="37832-119">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="37832-119">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="37832-120">Essa configuração de política permite controlar como as unidades de dados fixas protegidas por BitLocker são recuperadas na ausência das credenciais necessárias.</span><span class="sxs-lookup"><span data-stu-id="37832-120">This policy setting allows you to control how BitLocker-protected fixed data drives are recovered in the absence of the required credentials.</span></span> <span data-ttu-id="37832-121">Essa configuração de política é aplicada quando você ativa o BitLocker.</span><span class="sxs-lookup"><span data-stu-id="37832-121">This policy setting is applied when you turn on BitLocker.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37832-122">Relações</span><span class="sxs-lookup"><span data-stu-id="37832-122">Relationships</span></span>
<span data-ttu-id="37832-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="37832-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37832-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37832-124">JSON Representation</span></span>
<span data-ttu-id="37832-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37832-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerFixedDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  }
}
```




