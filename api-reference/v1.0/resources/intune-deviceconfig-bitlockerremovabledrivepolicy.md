---
title: Tipo de recurso bitLockerRemovableDrivePolicy
description: Políticas da unidade removível do BitLocker.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d10a1039c0186238504836c0f719ab19ae4c4882
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575069"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="ec8b3-103">Tipo de recurso bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="ec8b3-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="ec8b3-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ec8b3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec8b3-105">Políticas da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="ec8b3-105">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="ec8b3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec8b3-106">Properties</span></span>
|<span data-ttu-id="ec8b3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec8b3-107">Property</span></span>|<span data-ttu-id="ec8b3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec8b3-108">Type</span></span>|<span data-ttu-id="ec8b3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec8b3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec8b3-110">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="ec8b3-110">encryptionMethod</span></span>|[<span data-ttu-id="ec8b3-111">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="ec8b3-111">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="ec8b3-112">Selecione o método de criptografia para unidades removíveis.</span><span class="sxs-lookup"><span data-stu-id="ec8b3-112">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="ec8b3-113">Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="ec8b3-113">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="ec8b3-114">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="ec8b3-114">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="ec8b3-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="ec8b3-115">Boolean</span></span>|<span data-ttu-id="ec8b3-116">Indica se o acesso de gravação deve ser bloqueado para dispositivos configurados em outra organização.</span><span class="sxs-lookup"><span data-stu-id="ec8b3-116">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="ec8b3-117">Se requireEncryptionForWriteAccess for false, esse valor não será afetado.</span><span class="sxs-lookup"><span data-stu-id="ec8b3-117">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="ec8b3-118">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="ec8b3-118">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="ec8b3-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="ec8b3-119">Boolean</span></span>|<span data-ttu-id="ec8b3-120">Essa configuração de política determina se a proteção BitLocker é necessária para que unidades de dados removíveis sejam graváveis em um computador.</span><span class="sxs-lookup"><span data-stu-id="ec8b3-120">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec8b3-121">Relações</span><span class="sxs-lookup"><span data-stu-id="ec8b3-121">Relationships</span></span>
<span data-ttu-id="ec8b3-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ec8b3-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec8b3-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec8b3-123">JSON Representation</span></span>
<span data-ttu-id="ec8b3-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ec8b3-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```



