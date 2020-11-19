---
title: tipo de recurso bitLockerFixedDrivePolicy
description: Políticas de unidade fixa do BitLocker.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 323d45fb8109820a74f6b0394431a297ed2618e6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260610"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a><span data-ttu-id="3ec3a-103">tipo de recurso bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="3ec3a-103">bitLockerFixedDrivePolicy resource type</span></span>

<span data-ttu-id="3ec3a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ec3a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ec3a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3ec3a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ec3a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3ec3a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ec3a-107">Políticas de unidade fixa do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="3ec3a-107">BitLocker Fixed Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="3ec3a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ec3a-108">Properties</span></span>
|<span data-ttu-id="3ec3a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ec3a-109">Property</span></span>|<span data-ttu-id="3ec3a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ec3a-110">Type</span></span>|<span data-ttu-id="3ec3a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ec3a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ec3a-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="3ec3a-112">encryptionMethod</span></span>|[<span data-ttu-id="3ec3a-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="3ec3a-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="3ec3a-114">Selecione o método de criptografia para unidades fixas.</span><span class="sxs-lookup"><span data-stu-id="3ec3a-114">Select the encryption method for fixed drives.</span></span> <span data-ttu-id="3ec3a-115">Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="3ec3a-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="3ec3a-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="3ec3a-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="3ec3a-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="3ec3a-117">Boolean</span></span>|<span data-ttu-id="3ec3a-118">Essa configuração de política determina se é necessário proteger o BitLocker para unidades de dados fixas em um computador.</span><span class="sxs-lookup"><span data-stu-id="3ec3a-118">This policy setting determines whether BitLocker protection is required for fixed data drives to be writable on a computer.</span></span>|
|<span data-ttu-id="3ec3a-119">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="3ec3a-119">recoveryOptions</span></span>|[<span data-ttu-id="3ec3a-120">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="3ec3a-120">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="3ec3a-121">Essa configuração de política permite controlar como as unidades de dados fixas protegidas por BitLocker são recuperadas na ausência das credenciais necessárias.</span><span class="sxs-lookup"><span data-stu-id="3ec3a-121">This policy setting allows you to control how BitLocker-protected fixed data drives are recovered in the absence of the required credentials.</span></span> <span data-ttu-id="3ec3a-122">Essa configuração de política é aplicada quando você ativa o BitLocker.</span><span class="sxs-lookup"><span data-stu-id="3ec3a-122">This policy setting is applied when you turn on BitLocker.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ec3a-123">Relações</span><span class="sxs-lookup"><span data-stu-id="3ec3a-123">Relationships</span></span>
<span data-ttu-id="3ec3a-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3ec3a-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ec3a-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ec3a-125">JSON Representation</span></span>
<span data-ttu-id="3ec3a-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3ec3a-126">Here is a JSON representation of the resource.</span></span>
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




