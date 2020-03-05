---
title: tipo de enumeração filevaultstate
description: Estado FileVault
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8f2fa72d2db91ba000209332aec3d59579cba822
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529995"
---
# <a name="filevaultstate-enum-type"></a><span data-ttu-id="00bc4-103">tipo de enumeração filevaultstate</span><span class="sxs-lookup"><span data-stu-id="00bc4-103">fileVaultState enum type</span></span>

<span data-ttu-id="00bc4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="00bc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00bc4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="00bc4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00bc4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="00bc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00bc4-107">Estado FileVault</span><span class="sxs-lookup"><span data-stu-id="00bc4-107">FileVault State</span></span>

## <a name="members"></a><span data-ttu-id="00bc4-108">Membros</span><span class="sxs-lookup"><span data-stu-id="00bc4-108">Members</span></span>
|<span data-ttu-id="00bc4-109">Membro</span><span class="sxs-lookup"><span data-stu-id="00bc4-109">Member</span></span>|<span data-ttu-id="00bc4-110">Valor</span><span class="sxs-lookup"><span data-stu-id="00bc4-110">Value</span></span>|<span data-ttu-id="00bc4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="00bc4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00bc4-112">sucesso</span><span class="sxs-lookup"><span data-stu-id="00bc4-112">success</span></span>|<span data-ttu-id="00bc4-113">,0</span><span class="sxs-lookup"><span data-stu-id="00bc4-113">0</span></span>|<span data-ttu-id="00bc4-114">Êxito no estado FileVault</span><span class="sxs-lookup"><span data-stu-id="00bc4-114">FileVault State Success</span></span>|
|<span data-ttu-id="00bc4-115">driveEncryptedByUser</span><span class="sxs-lookup"><span data-stu-id="00bc4-115">driveEncryptedByUser</span></span>|<span data-ttu-id="00bc4-116">1 </span><span class="sxs-lookup"><span data-stu-id="00bc4-116">1</span></span>|<span data-ttu-id="00bc4-117">O FileVault foi habilitado pelo usuário e não está sendo gerenciado por política</span><span class="sxs-lookup"><span data-stu-id="00bc4-117">FileVault has been enabled by user and is not being managed by policy</span></span>|
|<span data-ttu-id="00bc4-118">userDeferredEncryption</span><span class="sxs-lookup"><span data-stu-id="00bc4-118">userDeferredEncryption</span></span>|<span data-ttu-id="00bc4-119">2 </span><span class="sxs-lookup"><span data-stu-id="00bc4-119">2</span></span>|<span data-ttu-id="00bc4-120">A política do FileVault foi instalada com êxito, mas o usuário não iniciou a criptografia</span><span class="sxs-lookup"><span data-stu-id="00bc4-120">FileVault policy is successfully installed but user has not started encryption</span></span>|
|<span data-ttu-id="00bc4-121">escrowNotEnabled</span><span class="sxs-lookup"><span data-stu-id="00bc4-121">escrowNotEnabled</span></span>|<span data-ttu-id="00bc4-122">4 </span><span class="sxs-lookup"><span data-stu-id="00bc4-122">4</span></span>|<span data-ttu-id="00bc4-123">A caução da chave de recuperação FileVault não está habilitada</span><span class="sxs-lookup"><span data-stu-id="00bc4-123">FileVault recovery key escrow is not enabled</span></span>|



