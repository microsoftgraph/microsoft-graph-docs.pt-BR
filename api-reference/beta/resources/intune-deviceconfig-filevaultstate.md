---
title: tipo de enumeração filevaultstate
description: Estado FileVault
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2d7f69413ac7fd4be1e857951b2a70aac0fe7bc3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444313"
---
# <a name="filevaultstate-enum-type"></a><span data-ttu-id="c56f7-103">tipo de enumeração filevaultstate</span><span class="sxs-lookup"><span data-stu-id="c56f7-103">fileVaultState enum type</span></span>

<span data-ttu-id="c56f7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c56f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c56f7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c56f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c56f7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c56f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c56f7-107">Estado FileVault</span><span class="sxs-lookup"><span data-stu-id="c56f7-107">FileVault State</span></span>

## <a name="members"></a><span data-ttu-id="c56f7-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c56f7-108">Members</span></span>
|<span data-ttu-id="c56f7-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c56f7-109">Member</span></span>|<span data-ttu-id="c56f7-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c56f7-110">Value</span></span>|<span data-ttu-id="c56f7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c56f7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c56f7-112">sucesso</span><span class="sxs-lookup"><span data-stu-id="c56f7-112">success</span></span>|<span data-ttu-id="c56f7-113">,0</span><span class="sxs-lookup"><span data-stu-id="c56f7-113">0</span></span>|<span data-ttu-id="c56f7-114">Êxito no estado FileVault</span><span class="sxs-lookup"><span data-stu-id="c56f7-114">FileVault State Success</span></span>|
|<span data-ttu-id="c56f7-115">driveEncryptedByUser</span><span class="sxs-lookup"><span data-stu-id="c56f7-115">driveEncryptedByUser</span></span>|<span data-ttu-id="c56f7-116">1</span><span class="sxs-lookup"><span data-stu-id="c56f7-116">1</span></span>|<span data-ttu-id="c56f7-117">O FileVault foi habilitado pelo usuário e não está sendo gerenciado por política</span><span class="sxs-lookup"><span data-stu-id="c56f7-117">FileVault has been enabled by user and is not being managed by policy</span></span>|
|<span data-ttu-id="c56f7-118">userDeferredEncryption</span><span class="sxs-lookup"><span data-stu-id="c56f7-118">userDeferredEncryption</span></span>|<span data-ttu-id="c56f7-119">duas</span><span class="sxs-lookup"><span data-stu-id="c56f7-119">2</span></span>|<span data-ttu-id="c56f7-120">A política do FileVault foi instalada com êxito, mas o usuário não iniciou a criptografia</span><span class="sxs-lookup"><span data-stu-id="c56f7-120">FileVault policy is successfully installed but user has not started encryption</span></span>|
|<span data-ttu-id="c56f7-121">escrowNotEnabled</span><span class="sxs-lookup"><span data-stu-id="c56f7-121">escrowNotEnabled</span></span>|<span data-ttu-id="c56f7-122">4 </span><span class="sxs-lookup"><span data-stu-id="c56f7-122">4</span></span>|<span data-ttu-id="c56f7-123">A caução da chave de recuperação FileVault não está habilitada</span><span class="sxs-lookup"><span data-stu-id="c56f7-123">FileVault recovery key escrow is not enabled</span></span>|



