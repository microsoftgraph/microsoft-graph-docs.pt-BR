---
title: Tipo de recurso bitLockerRemovableDrivePolicy
description: Políticas da unidade removível do BitLocker.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 040f4230cf1d3aab02f97237b88093126f8dc24c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926334"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="a5854-103">Tipo de recurso bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="a5854-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="a5854-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a5854-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5854-105">Políticas da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="a5854-105">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="a5854-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a5854-106">Properties</span></span>
|<span data-ttu-id="a5854-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5854-107">Property</span></span>|<span data-ttu-id="a5854-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5854-108">Type</span></span>|<span data-ttu-id="a5854-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5854-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5854-110">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="a5854-110">encryptionMethod</span></span>|[<span data-ttu-id="a5854-111">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="a5854-111">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="a5854-112">Selecione o método de criptografia para unidades removíveis.</span><span class="sxs-lookup"><span data-stu-id="a5854-112">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="a5854-113">Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="a5854-113">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="a5854-114">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="a5854-114">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="a5854-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="a5854-115">Boolean</span></span>|<span data-ttu-id="a5854-116">Indica se o acesso de gravação deve ser bloqueado para dispositivos configurados em outra organização.</span><span class="sxs-lookup"><span data-stu-id="a5854-116">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="a5854-117">Se requireEncryptionForWriteAccess for false, esse valor não será afetado.</span><span class="sxs-lookup"><span data-stu-id="a5854-117">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="a5854-118">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="a5854-118">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="a5854-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="a5854-119">Boolean</span></span>|<span data-ttu-id="a5854-120">Essa configuração de política determina se a proteção BitLocker é necessária para que unidades de dados removíveis sejam graváveis em um computador.</span><span class="sxs-lookup"><span data-stu-id="a5854-120">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5854-121">Relações</span><span class="sxs-lookup"><span data-stu-id="a5854-121">Relationships</span></span>
<span data-ttu-id="a5854-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a5854-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a5854-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a5854-123">JSON Representation</span></span>
<span data-ttu-id="a5854-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a5854-124">Here is a JSON representation of the resource.</span></span>
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



