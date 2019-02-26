---
title: Tipo de recurso bitLockerRemovableDrivePolicy
description: Políticas da unidade removível do BitLocker.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e7e343fc32af61b38c1cd14cf1fba29de549e99
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149424"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="4e196-103">Tipo de recurso bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="4e196-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="4e196-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4e196-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e196-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e196-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e196-106">Políticas da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="4e196-106">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="4e196-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e196-107">Properties</span></span>
|<span data-ttu-id="4e196-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e196-108">Property</span></span>|<span data-ttu-id="4e196-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e196-109">Type</span></span>|<span data-ttu-id="4e196-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e196-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e196-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="4e196-111">encryptionMethod</span></span>|[<span data-ttu-id="4e196-112">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="4e196-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="4e196-113">Selecione o método de criptografia para unidades removíveis.</span><span class="sxs-lookup"><span data-stu-id="4e196-113">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="4e196-114">Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="4e196-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="4e196-115">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="4e196-115">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="4e196-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e196-116">Boolean</span></span>|<span data-ttu-id="4e196-117">Indica se o acesso de gravação deve ser bloqueado para dispositivos configurados em outra organização.</span><span class="sxs-lookup"><span data-stu-id="4e196-117">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="4e196-118">Se requireEncryptionForWriteAccess for false, esse valor não será afetado.</span><span class="sxs-lookup"><span data-stu-id="4e196-118">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="4e196-119">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="4e196-119">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="4e196-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="4e196-120">Boolean</span></span>|<span data-ttu-id="4e196-121">Essa configuração de política determina se a proteção BitLocker é necessária para que unidades de dados removíveis sejam graváveis em um computador.</span><span class="sxs-lookup"><span data-stu-id="4e196-121">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e196-122">Relações</span><span class="sxs-lookup"><span data-stu-id="4e196-122">Relationships</span></span>
<span data-ttu-id="4e196-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4e196-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e196-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e196-124">JSON Representation</span></span>
<span data-ttu-id="4e196-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e196-125">Here is a JSON representation of the resource.</span></span>
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




