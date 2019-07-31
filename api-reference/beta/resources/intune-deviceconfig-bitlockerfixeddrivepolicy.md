---
title: tipo de recurso bitLockerFixedDrivePolicy
description: Políticas de unidade fixa do BitLocker.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3269fb0865f8cf08a4dbade3d949701b027b84fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971085"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a><span data-ttu-id="a5cfd-103">tipo de recurso bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="a5cfd-103">bitLockerFixedDrivePolicy resource type</span></span>

> <span data-ttu-id="a5cfd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a5cfd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5cfd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a5cfd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5cfd-106">Políticas de unidade fixa do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="a5cfd-106">BitLocker Fixed Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="a5cfd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a5cfd-107">Properties</span></span>
|<span data-ttu-id="a5cfd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5cfd-108">Property</span></span>|<span data-ttu-id="a5cfd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5cfd-109">Type</span></span>|<span data-ttu-id="a5cfd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5cfd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5cfd-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="a5cfd-111">encryptionMethod</span></span>|[<span data-ttu-id="a5cfd-112">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="a5cfd-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="a5cfd-113">Selecione o método de criptografia para unidades fixas.</span><span class="sxs-lookup"><span data-stu-id="a5cfd-113">Select the encryption method for fixed drives.</span></span> <span data-ttu-id="a5cfd-114">Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="a5cfd-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="a5cfd-115">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="a5cfd-115">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="a5cfd-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="a5cfd-116">Boolean</span></span>|<span data-ttu-id="a5cfd-117">Essa configuração de política determina se é necessário proteger o BitLocker para unidades de dados fixas em um computador.</span><span class="sxs-lookup"><span data-stu-id="a5cfd-117">This policy setting determines whether BitLocker protection is required for fixed data drives to be writable on a computer.</span></span>|
|<span data-ttu-id="a5cfd-118">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="a5cfd-118">recoveryOptions</span></span>|[<span data-ttu-id="a5cfd-119">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="a5cfd-119">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="a5cfd-120">Essa configuração de política permite controlar como as unidades de dados fixas protegidas por BitLocker são recuperadas na ausência das credenciais necessárias.</span><span class="sxs-lookup"><span data-stu-id="a5cfd-120">This policy setting allows you to control how BitLocker-protected fixed data drives are recovered in the absence of the required credentials.</span></span> <span data-ttu-id="a5cfd-121">Essa configuração de política é aplicada quando você ativa o BitLocker.</span><span class="sxs-lookup"><span data-stu-id="a5cfd-121">This policy setting is applied when you turn on BitLocker.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5cfd-122">Relações</span><span class="sxs-lookup"><span data-stu-id="a5cfd-122">Relationships</span></span>
<span data-ttu-id="a5cfd-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a5cfd-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5cfd-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a5cfd-124">JSON Representation</span></span>
<span data-ttu-id="a5cfd-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a5cfd-125">Here is a JSON representation of the resource.</span></span>
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





