---
title: tipo de recurso de bitLockerFixedDrivePolicy
description: O BitLocker fixa políticas de unidade.
ms.openlocfilehash: c29f736515333fcdbeca8c18017b9403f845de9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036974"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a><span data-ttu-id="162f2-103">tipo de recurso de bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="162f2-103">bitLockerFixedDrivePolicy resource type</span></span>

> <span data-ttu-id="162f2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="162f2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="162f2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="162f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="162f2-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="162f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="162f2-107">O BitLocker fixa políticas de unidade.</span><span class="sxs-lookup"><span data-stu-id="162f2-107">BitLocker Fixed Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="162f2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="162f2-108">Properties</span></span>
|<span data-ttu-id="162f2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="162f2-109">Property</span></span>|<span data-ttu-id="162f2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="162f2-110">Type</span></span>|<span data-ttu-id="162f2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="162f2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="162f2-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="162f2-112">encryptionMethod</span></span>|[<span data-ttu-id="162f2-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="162f2-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="162f2-114">Selecione o método de criptografia para unidades fixas.</span><span class="sxs-lookup"><span data-stu-id="162f2-114">Select the encryption method for fixed drives.</span></span> <span data-ttu-id="162f2-115">Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="162f2-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="162f2-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="162f2-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="162f2-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="162f2-117">Boolean</span></span>|<span data-ttu-id="162f2-118">Essa configuração de diretiva determina se a proteção BitLocker é necessária para unidades de dados fixas ser gravado em um computador.</span><span class="sxs-lookup"><span data-stu-id="162f2-118">This policy setting determines whether BitLocker protection is required for fixed data drives to be writable on a computer.</span></span>|
|<span data-ttu-id="162f2-119">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="162f2-119">recoveryOptions</span></span>|[<span data-ttu-id="162f2-120">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="162f2-120">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="162f2-121">Essa configuração de política permite que você controle de dados fixo como protegidas pelo BitLocker unidades são recuperadas na ausência das credenciais necessárias.</span><span class="sxs-lookup"><span data-stu-id="162f2-121">This policy setting allows you to control how BitLocker-protected fixed data drives are recovered in the absence of the required credentials.</span></span> <span data-ttu-id="162f2-122">Essa configuração de política é aplicada quando você ativa o BitLocker.</span><span class="sxs-lookup"><span data-stu-id="162f2-122">This policy setting is applied when you turn on BitLocker.</span></span>|

## <a name="relationships"></a><span data-ttu-id="162f2-123">Relações</span><span class="sxs-lookup"><span data-stu-id="162f2-123">Relationships</span></span>
<span data-ttu-id="162f2-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="162f2-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="162f2-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="162f2-125">JSON Representation</span></span>
<span data-ttu-id="162f2-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="162f2-126">Here is a JSON representation of the resource.</span></span>
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





