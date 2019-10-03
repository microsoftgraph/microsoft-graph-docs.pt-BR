---
title: Tipo de recurso bitLockerRemovableDrivePolicy
description: Políticas da unidade removível do BitLocker.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ab8c77f0581f33f3fa68640647808c43acb8eeec
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366661"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="3e87e-103">Tipo de recurso bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="3e87e-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="3e87e-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3e87e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e87e-105">Políticas da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="3e87e-105">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="3e87e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e87e-106">Properties</span></span>
|<span data-ttu-id="3e87e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e87e-107">Property</span></span>|<span data-ttu-id="3e87e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e87e-108">Type</span></span>|<span data-ttu-id="3e87e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e87e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e87e-110">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="3e87e-110">encryptionMethod</span></span>|[<span data-ttu-id="3e87e-111">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="3e87e-111">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="3e87e-112">Selecione o método de criptografia para unidades removíveis.</span><span class="sxs-lookup"><span data-stu-id="3e87e-112">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="3e87e-113">Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="3e87e-113">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="3e87e-114">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="3e87e-114">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="3e87e-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="3e87e-115">Boolean</span></span>|<span data-ttu-id="3e87e-116">Indica se o acesso de gravação deve ser bloqueado para dispositivos configurados em outra organização.</span><span class="sxs-lookup"><span data-stu-id="3e87e-116">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="3e87e-117">Se requireEncryptionForWriteAccess for false, esse valor não será afetado.</span><span class="sxs-lookup"><span data-stu-id="3e87e-117">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="3e87e-118">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="3e87e-118">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="3e87e-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="3e87e-119">Boolean</span></span>|<span data-ttu-id="3e87e-120">Essa configuração de política determina se a proteção BitLocker é necessária para que unidades de dados removíveis sejam graváveis em um computador.</span><span class="sxs-lookup"><span data-stu-id="3e87e-120">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e87e-121">Relações</span><span class="sxs-lookup"><span data-stu-id="3e87e-121">Relationships</span></span>
<span data-ttu-id="3e87e-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3e87e-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e87e-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e87e-123">JSON Representation</span></span>
<span data-ttu-id="3e87e-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e87e-124">Here is a JSON representation of the resource.</span></span>
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




