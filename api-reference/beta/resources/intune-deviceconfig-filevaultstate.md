---
title: tipo de enumeração filevaultstate
description: Estado FileVault
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c1ef23c9428b2d8b5ed82c5264d829eb0b1febde
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734032"
---
# <a name="filevaultstate-enum-type"></a><span data-ttu-id="d9027-103">tipo de enumeração filevaultstate</span><span class="sxs-lookup"><span data-stu-id="d9027-103">fileVaultState enum type</span></span>

<span data-ttu-id="d9027-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9027-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9027-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9027-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9027-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9027-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9027-107">Estado FileVault</span><span class="sxs-lookup"><span data-stu-id="d9027-107">FileVault State</span></span>

## <a name="members"></a><span data-ttu-id="d9027-108">Membros</span><span class="sxs-lookup"><span data-stu-id="d9027-108">Members</span></span>
|<span data-ttu-id="d9027-109">Membro</span><span class="sxs-lookup"><span data-stu-id="d9027-109">Member</span></span>|<span data-ttu-id="d9027-110">Valor</span><span class="sxs-lookup"><span data-stu-id="d9027-110">Value</span></span>|<span data-ttu-id="d9027-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9027-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9027-112">sucesso</span><span class="sxs-lookup"><span data-stu-id="d9027-112">success</span></span>|<span data-ttu-id="d9027-113">,0</span><span class="sxs-lookup"><span data-stu-id="d9027-113">0</span></span>|<span data-ttu-id="d9027-114">Êxito no estado FileVault</span><span class="sxs-lookup"><span data-stu-id="d9027-114">FileVault State Success</span></span>|
|<span data-ttu-id="d9027-115">driveEncryptedByUser</span><span class="sxs-lookup"><span data-stu-id="d9027-115">driveEncryptedByUser</span></span>|<span data-ttu-id="d9027-116">1</span><span class="sxs-lookup"><span data-stu-id="d9027-116">1</span></span>|<span data-ttu-id="d9027-117">O FileVault foi habilitado pelo usuário e não está sendo gerenciado por política</span><span class="sxs-lookup"><span data-stu-id="d9027-117">FileVault has been enabled by user and is not being managed by policy</span></span>|
|<span data-ttu-id="d9027-118">userDeferredEncryption</span><span class="sxs-lookup"><span data-stu-id="d9027-118">userDeferredEncryption</span></span>|<span data-ttu-id="d9027-119">duas</span><span class="sxs-lookup"><span data-stu-id="d9027-119">2</span></span>|<span data-ttu-id="d9027-120">A política do FileVault foi instalada com êxito, mas o usuário não iniciou a criptografia</span><span class="sxs-lookup"><span data-stu-id="d9027-120">FileVault policy is successfully installed but user has not started encryption</span></span>|
|<span data-ttu-id="d9027-121">escrowNotEnabled</span><span class="sxs-lookup"><span data-stu-id="d9027-121">escrowNotEnabled</span></span>|<span data-ttu-id="d9027-122">4 </span><span class="sxs-lookup"><span data-stu-id="d9027-122">4</span></span>|<span data-ttu-id="d9027-123">A caução da chave de recuperação FileVault não está habilitada</span><span class="sxs-lookup"><span data-stu-id="d9027-123">FileVault recovery key escrow is not enabled</span></span>|





