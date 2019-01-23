---
title: Tipo de recurso bitLockerRemovableDrivePolicy
description: Políticas da unidade removível do BitLocker.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 57a3ad19e988327e126b6da757c2dc5b90c280de
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425614"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="2e306-103">Tipo de recurso bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="2e306-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="2e306-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="2e306-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2e306-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2e306-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2e306-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="2e306-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e306-107">Políticas da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="2e306-107">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="2e306-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2e306-108">Properties</span></span>
|<span data-ttu-id="2e306-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e306-109">Property</span></span>|<span data-ttu-id="2e306-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e306-110">Type</span></span>|<span data-ttu-id="2e306-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e306-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e306-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="2e306-112">encryptionMethod</span></span>|[<span data-ttu-id="2e306-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="2e306-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="2e306-114">Selecione o método de criptografia para unidades removíveis.</span><span class="sxs-lookup"><span data-stu-id="2e306-114">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="2e306-115">Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="2e306-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="2e306-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="2e306-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="2e306-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="2e306-117">Boolean</span></span>|<span data-ttu-id="2e306-118">Indica se o acesso de gravação deve ser bloqueado para dispositivos configurados em outra organização.</span><span class="sxs-lookup"><span data-stu-id="2e306-118">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="2e306-119">Se requireEncryptionForWriteAccess for false, esse valor não será afetado.</span><span class="sxs-lookup"><span data-stu-id="2e306-119">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="2e306-120">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="2e306-120">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="2e306-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="2e306-121">Boolean</span></span>|<span data-ttu-id="2e306-122">Essa configuração de política determina se a proteção BitLocker é necessária para que unidades de dados removíveis sejam graváveis em um computador.</span><span class="sxs-lookup"><span data-stu-id="2e306-122">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e306-123">Relações</span><span class="sxs-lookup"><span data-stu-id="2e306-123">Relationships</span></span>
<span data-ttu-id="2e306-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2e306-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e306-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2e306-125">JSON Representation</span></span>
<span data-ttu-id="2e306-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2e306-126">Here is a JSON representation of the resource.</span></span>
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




