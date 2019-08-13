---
title: tipo de enumeração filevaultstate
description: Estado FileVault
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 54e8076dc4b4f6ab20f7790d2a650de6c07aa702
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325565"
---
# <a name="filevaultstate-enum-type"></a><span data-ttu-id="cb828-103">tipo de enumeração filevaultstate</span><span class="sxs-lookup"><span data-stu-id="cb828-103">fileVaultState enum type</span></span>

> <span data-ttu-id="cb828-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cb828-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb828-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cb828-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb828-106">Estado FileVault</span><span class="sxs-lookup"><span data-stu-id="cb828-106">FileVault State</span></span>

## <a name="members"></a><span data-ttu-id="cb828-107">Membros</span><span class="sxs-lookup"><span data-stu-id="cb828-107">Members</span></span>
|<span data-ttu-id="cb828-108">Membro</span><span class="sxs-lookup"><span data-stu-id="cb828-108">Member</span></span>|<span data-ttu-id="cb828-109">Valor</span><span class="sxs-lookup"><span data-stu-id="cb828-109">Value</span></span>|<span data-ttu-id="cb828-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb828-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb828-111">sucesso</span><span class="sxs-lookup"><span data-stu-id="cb828-111">success</span></span>|<span data-ttu-id="cb828-112">,0</span><span class="sxs-lookup"><span data-stu-id="cb828-112">0</span></span>|<span data-ttu-id="cb828-113">Êxito no estado FileVault</span><span class="sxs-lookup"><span data-stu-id="cb828-113">FileVault State Success</span></span>|
|<span data-ttu-id="cb828-114">driveEncryptedByUser</span><span class="sxs-lookup"><span data-stu-id="cb828-114">driveEncryptedByUser</span></span>|<span data-ttu-id="cb828-115">1</span><span class="sxs-lookup"><span data-stu-id="cb828-115">1</span></span>|<span data-ttu-id="cb828-116">O FileVault foi habilitado pelo usuário e não está sendo gerenciado por política</span><span class="sxs-lookup"><span data-stu-id="cb828-116">FileVault has been enabled by user and is not being managed by policy</span></span>|
|<span data-ttu-id="cb828-117">userDeferredEncryption</span><span class="sxs-lookup"><span data-stu-id="cb828-117">userDeferredEncryption</span></span>|<span data-ttu-id="cb828-118">duas</span><span class="sxs-lookup"><span data-stu-id="cb828-118">2</span></span>|<span data-ttu-id="cb828-119">A política do FileVault foi instalada com êxito, mas o usuário não iniciou a criptografia</span><span class="sxs-lookup"><span data-stu-id="cb828-119">FileVault policy is successfully installed but user has not started encryption</span></span>|
|<span data-ttu-id="cb828-120">escrowNotEnabled</span><span class="sxs-lookup"><span data-stu-id="cb828-120">escrowNotEnabled</span></span>|<span data-ttu-id="cb828-121">quatro</span><span class="sxs-lookup"><span data-stu-id="cb828-121">4</span></span>|<span data-ttu-id="cb828-122">A caução da chave de recuperação FileVault não está habilitada</span><span class="sxs-lookup"><span data-stu-id="cb828-122">FileVault recovery key escrow is not enabled</span></span>|



