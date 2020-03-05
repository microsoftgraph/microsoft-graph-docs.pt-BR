---
title: Tipo de recurso bitLockerRemovableDrivePolicy
description: Políticas da unidade removível do BitLocker.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 90d1bcb5464b6fbd1d31d0ddbc3f2bbd525d80d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527018"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="d2d72-103">Tipo de recurso bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d2d72-103">bitLockerRemovableDrivePolicy resource type</span></span>

<span data-ttu-id="d2d72-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d2d72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2d72-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d2d72-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2d72-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d2d72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2d72-107">Políticas da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d2d72-107">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="d2d72-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2d72-108">Properties</span></span>
|<span data-ttu-id="d2d72-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2d72-109">Property</span></span>|<span data-ttu-id="d2d72-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2d72-110">Type</span></span>|<span data-ttu-id="d2d72-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2d72-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2d72-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="d2d72-112">encryptionMethod</span></span>|[<span data-ttu-id="d2d72-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="d2d72-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="d2d72-114">Selecione o método de criptografia para unidades removíveis.</span><span class="sxs-lookup"><span data-stu-id="d2d72-114">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="d2d72-115">Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="d2d72-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="d2d72-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="d2d72-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="d2d72-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2d72-117">Boolean</span></span>|<span data-ttu-id="d2d72-118">Indica se o acesso de gravação deve ser bloqueado para dispositivos configurados em outra organização.</span><span class="sxs-lookup"><span data-stu-id="d2d72-118">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="d2d72-119">Se requireEncryptionForWriteAccess for false, esse valor não será afetado.</span><span class="sxs-lookup"><span data-stu-id="d2d72-119">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="d2d72-120">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="d2d72-120">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="d2d72-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="d2d72-121">Boolean</span></span>|<span data-ttu-id="d2d72-122">Essa configuração de política determina se a proteção BitLocker é necessária para que unidades de dados removíveis sejam graváveis em um computador.</span><span class="sxs-lookup"><span data-stu-id="d2d72-122">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2d72-123">Relações</span><span class="sxs-lookup"><span data-stu-id="d2d72-123">Relationships</span></span>
<span data-ttu-id="d2d72-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2d72-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2d72-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2d72-125">JSON Representation</span></span>
<span data-ttu-id="d2d72-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2d72-126">Here is a JSON representation of the resource.</span></span>
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



