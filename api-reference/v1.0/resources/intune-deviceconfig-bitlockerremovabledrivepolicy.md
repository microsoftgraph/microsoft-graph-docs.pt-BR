---
title: Tipo de recurso bitLockerRemovableDrivePolicy
description: Políticas da unidade removível do BitLocker.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 254a57d8da1bd6940096377de0bbc183b6893197
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760262"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="d5fa7-103">Tipo de recurso bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d5fa7-103">bitLockerRemovableDrivePolicy resource type</span></span>

<span data-ttu-id="d5fa7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5fa7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5fa7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d5fa7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5fa7-106">Políticas da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d5fa7-106">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="d5fa7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5fa7-107">Properties</span></span>
|<span data-ttu-id="d5fa7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5fa7-108">Property</span></span>|<span data-ttu-id="d5fa7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5fa7-109">Type</span></span>|<span data-ttu-id="d5fa7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5fa7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5fa7-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="d5fa7-111">encryptionMethod</span></span>|[<span data-ttu-id="d5fa7-112">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="d5fa7-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="d5fa7-113">Selecione o método de criptografia para unidades removíveis.</span><span class="sxs-lookup"><span data-stu-id="d5fa7-113">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="d5fa7-114">Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="d5fa7-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="d5fa7-115">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="d5fa7-115">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="d5fa7-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="d5fa7-116">Boolean</span></span>|<span data-ttu-id="d5fa7-117">Indica se o acesso de gravação deve ser bloqueado para dispositivos configurados em outra organização.</span><span class="sxs-lookup"><span data-stu-id="d5fa7-117">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="d5fa7-118">Se requireEncryptionForWriteAccess for false, esse valor não será afetado.</span><span class="sxs-lookup"><span data-stu-id="d5fa7-118">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="d5fa7-119">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="d5fa7-119">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="d5fa7-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="d5fa7-120">Boolean</span></span>|<span data-ttu-id="d5fa7-121">Essa configuração de política determina se a proteção BitLocker é necessária para que unidades de dados removíveis sejam graváveis em um computador.</span><span class="sxs-lookup"><span data-stu-id="d5fa7-121">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5fa7-122">Relações</span><span class="sxs-lookup"><span data-stu-id="d5fa7-122">Relationships</span></span>
<span data-ttu-id="d5fa7-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5fa7-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5fa7-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5fa7-124">JSON Representation</span></span>
<span data-ttu-id="d5fa7-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5fa7-125">Here is a JSON representation of the resource.</span></span>
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




