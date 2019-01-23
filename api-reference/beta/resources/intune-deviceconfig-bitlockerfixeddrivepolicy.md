---
title: tipo de recurso de bitLockerFixedDrivePolicy
description: O BitLocker fixa políticas de unidade.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8f233e4c1779a860cc40dc97007aa0216795928f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424662"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a><span data-ttu-id="a3511-103">tipo de recurso de bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="a3511-103">bitLockerFixedDrivePolicy resource type</span></span>

> <span data-ttu-id="a3511-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="a3511-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a3511-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a3511-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3511-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="a3511-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3511-107">O BitLocker fixa políticas de unidade.</span><span class="sxs-lookup"><span data-stu-id="a3511-107">BitLocker Fixed Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="a3511-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a3511-108">Properties</span></span>
|<span data-ttu-id="a3511-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3511-109">Property</span></span>|<span data-ttu-id="a3511-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3511-110">Type</span></span>|<span data-ttu-id="a3511-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3511-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3511-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="a3511-112">encryptionMethod</span></span>|[<span data-ttu-id="a3511-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="a3511-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="a3511-114">Selecione o método de criptografia para unidades fixas.</span><span class="sxs-lookup"><span data-stu-id="a3511-114">Select the encryption method for fixed drives.</span></span> <span data-ttu-id="a3511-115">Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="a3511-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="a3511-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="a3511-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="a3511-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="a3511-117">Boolean</span></span>|<span data-ttu-id="a3511-118">Essa configuração de diretiva determina se a proteção BitLocker é necessária para unidades de dados fixas ser gravado em um computador.</span><span class="sxs-lookup"><span data-stu-id="a3511-118">This policy setting determines whether BitLocker protection is required for fixed data drives to be writable on a computer.</span></span>|
|<span data-ttu-id="a3511-119">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="a3511-119">recoveryOptions</span></span>|[<span data-ttu-id="a3511-120">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="a3511-120">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="a3511-121">Essa configuração de política permite que você controle de dados fixo como protegidas pelo BitLocker unidades são recuperadas na ausência das credenciais necessárias.</span><span class="sxs-lookup"><span data-stu-id="a3511-121">This policy setting allows you to control how BitLocker-protected fixed data drives are recovered in the absence of the required credentials.</span></span> <span data-ttu-id="a3511-122">Essa configuração de política é aplicada quando você ativa o BitLocker.</span><span class="sxs-lookup"><span data-stu-id="a3511-122">This policy setting is applied when you turn on BitLocker.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3511-123">Relações</span><span class="sxs-lookup"><span data-stu-id="a3511-123">Relationships</span></span>
<span data-ttu-id="a3511-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a3511-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3511-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a3511-125">JSON Representation</span></span>
<span data-ttu-id="a3511-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a3511-126">Here is a JSON representation of the resource.</span></span>
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




