---
title: tipo de enumeração filevaultstate
description: Estado FileVault
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f122d62f85f90825f5fe3129ec2a314d5886e6f2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725865"
---
# <a name="filevaultstate-enum-type"></a><span data-ttu-id="c7e30-103">tipo de enumeração filevaultstate</span><span class="sxs-lookup"><span data-stu-id="c7e30-103">fileVaultState enum type</span></span>

> <span data-ttu-id="c7e30-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7e30-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7e30-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7e30-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7e30-106">Estado FileVault</span><span class="sxs-lookup"><span data-stu-id="c7e30-106">FileVault State</span></span>

## <a name="members"></a><span data-ttu-id="c7e30-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c7e30-107">Members</span></span>
|<span data-ttu-id="c7e30-108">Membro</span><span class="sxs-lookup"><span data-stu-id="c7e30-108">Member</span></span>|<span data-ttu-id="c7e30-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c7e30-109">Value</span></span>|<span data-ttu-id="c7e30-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7e30-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7e30-111">sucesso</span><span class="sxs-lookup"><span data-stu-id="c7e30-111">success</span></span>|<span data-ttu-id="c7e30-112">,0</span><span class="sxs-lookup"><span data-stu-id="c7e30-112">0</span></span>|<span data-ttu-id="c7e30-113">Êxito no estado FileVault</span><span class="sxs-lookup"><span data-stu-id="c7e30-113">FileVault State Success</span></span>|
|<span data-ttu-id="c7e30-114">driveEncryptedByUser</span><span class="sxs-lookup"><span data-stu-id="c7e30-114">driveEncryptedByUser</span></span>|<span data-ttu-id="c7e30-115">1</span><span class="sxs-lookup"><span data-stu-id="c7e30-115">1</span></span>|<span data-ttu-id="c7e30-116">O FileVault foi habilitado pelo usuário e não está sendo gerenciado por política</span><span class="sxs-lookup"><span data-stu-id="c7e30-116">FileVault has been enabled by user and is not being managed by policy</span></span>|
|<span data-ttu-id="c7e30-117">userDeferredEncryption</span><span class="sxs-lookup"><span data-stu-id="c7e30-117">userDeferredEncryption</span></span>|<span data-ttu-id="c7e30-118">duas</span><span class="sxs-lookup"><span data-stu-id="c7e30-118">2</span></span>|<span data-ttu-id="c7e30-119">A política do FileVault foi instalada com êxito, mas o usuário não iniciou a criptografia</span><span class="sxs-lookup"><span data-stu-id="c7e30-119">FileVault policy is successfully installed but user has not started encryption</span></span>|
|<span data-ttu-id="c7e30-120">escrowNotEnabled</span><span class="sxs-lookup"><span data-stu-id="c7e30-120">escrowNotEnabled</span></span>|<span data-ttu-id="c7e30-121">quatro</span><span class="sxs-lookup"><span data-stu-id="c7e30-121">4</span></span>|<span data-ttu-id="c7e30-122">A caução da chave de recuperação FileVault não está habilitada</span><span class="sxs-lookup"><span data-stu-id="c7e30-122">FileVault recovery key escrow is not enabled</span></span>|







