---
title: Tipo de recurso bitLockerRemovableDrivePolicy
description: Políticas da unidade removível do BitLocker.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c5c474dc113d7d00bb0a43bef59c8196befddea3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028536"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="9dabc-103">Tipo de recurso bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="9dabc-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="9dabc-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9dabc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9dabc-105">Políticas da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="9dabc-105">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="9dabc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9dabc-106">Properties</span></span>
|<span data-ttu-id="9dabc-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9dabc-107">Property</span></span>|<span data-ttu-id="9dabc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9dabc-108">Type</span></span>|<span data-ttu-id="9dabc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9dabc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dabc-110">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="9dabc-110">encryptionMethod</span></span>|[<span data-ttu-id="9dabc-111">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="9dabc-111">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="9dabc-112">Selecione o método de criptografia para unidades removíveis.</span><span class="sxs-lookup"><span data-stu-id="9dabc-112">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="9dabc-113">Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="9dabc-113">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="9dabc-114">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="9dabc-114">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="9dabc-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="9dabc-115">Boolean</span></span>|<span data-ttu-id="9dabc-116">Indica se o acesso de gravação deve ser bloqueado para dispositivos configurados em outra organização.</span><span class="sxs-lookup"><span data-stu-id="9dabc-116">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="9dabc-117">Se requireEncryptionForWriteAccess for false, esse valor não será afetado.</span><span class="sxs-lookup"><span data-stu-id="9dabc-117">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="9dabc-118">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="9dabc-118">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="9dabc-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="9dabc-119">Boolean</span></span>|<span data-ttu-id="9dabc-120">Essa configuração de política determina se a proteção BitLocker é necessária para que unidades de dados removíveis sejam graváveis em um computador.</span><span class="sxs-lookup"><span data-stu-id="9dabc-120">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9dabc-121">Relações</span><span class="sxs-lookup"><span data-stu-id="9dabc-121">Relationships</span></span>
<span data-ttu-id="9dabc-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9dabc-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9dabc-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9dabc-123">JSON Representation</span></span>
<span data-ttu-id="9dabc-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9dabc-124">Here is a JSON representation of the resource.</span></span>
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



