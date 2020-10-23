---
title: tipo de enumeração macOSFileVaultRecoveryKeyTypes
description: Tipos de chave de recuperação para macOS FileVault
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 75d6de635ecddf44ce7eaa5f0c731af59125a7d0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724569"
---
# <a name="macosfilevaultrecoverykeytypes-enum-type"></a><span data-ttu-id="6d73b-103">tipo de enumeração macOSFileVaultRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="6d73b-103">macOSFileVaultRecoveryKeyTypes enum type</span></span>

<span data-ttu-id="6d73b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d73b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d73b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6d73b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d73b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d73b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d73b-107">Tipos de chave de recuperação para macOS FileVault</span><span class="sxs-lookup"><span data-stu-id="6d73b-107">Recovery key types for macOS FileVault</span></span>

## <a name="members"></a><span data-ttu-id="6d73b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6d73b-108">Members</span></span>
|<span data-ttu-id="6d73b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6d73b-109">Member</span></span>|<span data-ttu-id="6d73b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6d73b-110">Value</span></span>|<span data-ttu-id="6d73b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d73b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d73b-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6d73b-112">notConfigured</span></span>|<span data-ttu-id="6d73b-113">,0</span><span class="sxs-lookup"><span data-stu-id="6d73b-113">0</span></span>|<span data-ttu-id="6d73b-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="6d73b-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="6d73b-115">institutionalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="6d73b-115">institutionalRecoveryKey</span></span>|<span data-ttu-id="6d73b-116">1</span><span class="sxs-lookup"><span data-stu-id="6d73b-116">1</span></span>|<span data-ttu-id="6d73b-117">Uma chave de recuperação institucional é como uma chave de recuperação "mestra" que pode ser usada para desbloquear qualquer dispositivo cuja senha tenha sido perdida.</span><span class="sxs-lookup"><span data-stu-id="6d73b-117">An institutional recovery key is like a “master” recovery key that can be used to unlock any device whose password has been lost.</span></span>|
|<span data-ttu-id="6d73b-118">personalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="6d73b-118">personalRecoveryKey</span></span>|<span data-ttu-id="6d73b-119">duas</span><span class="sxs-lookup"><span data-stu-id="6d73b-119">2</span></span>|<span data-ttu-id="6d73b-120">Uma chave de recuperação pessoal é um código exclusivo que pode ser usado para desbloquear o dispositivo do usuário, mesmo se a senha do dispositivo for perdida.</span><span class="sxs-lookup"><span data-stu-id="6d73b-120">A personal recovery key is a unique code that can be used to unlock the user’s device, even if the password to the device is lost.</span></span>|





