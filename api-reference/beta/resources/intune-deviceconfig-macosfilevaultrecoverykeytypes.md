---
title: tipo de enumeração macOSFileVaultRecoveryKeyTypes
description: Tipos de chave de recuperação para macOS FileVault
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 77fe5f115fec13498d0dbd034d87872f65bfc211
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43383451"
---
# <a name="macosfilevaultrecoverykeytypes-enum-type"></a><span data-ttu-id="cb0f4-103">tipo de enumeração macOSFileVaultRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="cb0f4-103">macOSFileVaultRecoveryKeyTypes enum type</span></span>

<span data-ttu-id="cb0f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb0f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb0f4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cb0f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb0f4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cb0f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb0f4-107">Tipos de chave de recuperação para macOS FileVault</span><span class="sxs-lookup"><span data-stu-id="cb0f4-107">Recovery key types for macOS FileVault</span></span>

## <a name="members"></a><span data-ttu-id="cb0f4-108">Membros</span><span class="sxs-lookup"><span data-stu-id="cb0f4-108">Members</span></span>
|<span data-ttu-id="cb0f4-109">Membro</span><span class="sxs-lookup"><span data-stu-id="cb0f4-109">Member</span></span>|<span data-ttu-id="cb0f4-110">Valor</span><span class="sxs-lookup"><span data-stu-id="cb0f4-110">Value</span></span>|<span data-ttu-id="cb0f4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb0f4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb0f4-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="cb0f4-112">notConfigured</span></span>|<span data-ttu-id="cb0f4-113">,0</span><span class="sxs-lookup"><span data-stu-id="cb0f4-113">0</span></span>|<span data-ttu-id="cb0f4-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="cb0f4-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="cb0f4-115">institutionalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="cb0f4-115">institutionalRecoveryKey</span></span>|<span data-ttu-id="cb0f4-116">1</span><span class="sxs-lookup"><span data-stu-id="cb0f4-116">1</span></span>|<span data-ttu-id="cb0f4-117">Uma chave de recuperação institucional é como uma chave de recuperação "mestra" que pode ser usada para desbloquear qualquer dispositivo cuja senha tenha sido perdida.</span><span class="sxs-lookup"><span data-stu-id="cb0f4-117">An institutional recovery key is like a “master” recovery key that can be used to unlock any device whose password has been lost.</span></span>|
|<span data-ttu-id="cb0f4-118">personalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="cb0f4-118">personalRecoveryKey</span></span>|<span data-ttu-id="cb0f4-119">duas</span><span class="sxs-lookup"><span data-stu-id="cb0f4-119">2</span></span>|<span data-ttu-id="cb0f4-120">Uma chave de recuperação pessoal é um código exclusivo que pode ser usado para desbloquear o dispositivo do usuário, mesmo se a senha do dispositivo for perdida.</span><span class="sxs-lookup"><span data-stu-id="cb0f4-120">A personal recovery key is a unique code that can be used to unlock the user’s device, even if the password to the device is lost.</span></span>|



