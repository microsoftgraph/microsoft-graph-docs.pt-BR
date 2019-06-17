---
title: tipo de enumeração macOSFileVaultRecoveryKeyTypes
description: Tipos de chave de recuperação para macOS FileVault
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 193bfc5769da2919f93df9beef38524a57bfece0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002543"
---
# <a name="macosfilevaultrecoverykeytypes-enum-type"></a><span data-ttu-id="8e104-103">tipo de enumeração macOSFileVaultRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="8e104-103">macOSFileVaultRecoveryKeyTypes enum type</span></span>

> <span data-ttu-id="8e104-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8e104-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e104-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e104-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e104-106">Tipos de chave de recuperação para macOS FileVault</span><span class="sxs-lookup"><span data-stu-id="8e104-106">Recovery key types for macOS FileVault</span></span>

## <a name="members"></a><span data-ttu-id="8e104-107">Membros</span><span class="sxs-lookup"><span data-stu-id="8e104-107">Members</span></span>
|<span data-ttu-id="8e104-108">Membro</span><span class="sxs-lookup"><span data-stu-id="8e104-108">Member</span></span>|<span data-ttu-id="8e104-109">Valor</span><span class="sxs-lookup"><span data-stu-id="8e104-109">Value</span></span>|<span data-ttu-id="8e104-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e104-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e104-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="8e104-111">notConfigured</span></span>|<span data-ttu-id="8e104-112">,0</span><span class="sxs-lookup"><span data-stu-id="8e104-112">0</span></span>|<span data-ttu-id="8e104-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="8e104-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="8e104-114">institutionalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="8e104-114">institutionalRecoveryKey</span></span>|<span data-ttu-id="8e104-115">1</span><span class="sxs-lookup"><span data-stu-id="8e104-115">1</span></span>|<span data-ttu-id="8e104-116">Uma chave de recuperação institucional é como uma chave de recuperação "mestra" que pode ser usada para desbloquear qualquer dispositivo cuja senha tenha sido perdida.</span><span class="sxs-lookup"><span data-stu-id="8e104-116">An institutional recovery key is like a “master” recovery key that can be used to unlock any device whose password has been lost.</span></span>|
|<span data-ttu-id="8e104-117">personalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="8e104-117">personalRecoveryKey</span></span>|<span data-ttu-id="8e104-118">duas</span><span class="sxs-lookup"><span data-stu-id="8e104-118">2</span></span>|<span data-ttu-id="8e104-119">Uma chave de recuperação pessoal é um código exclusivo que pode ser usado para desbloquear o dispositivo do usuário, mesmo se a senha do dispositivo for perdida.</span><span class="sxs-lookup"><span data-stu-id="8e104-119">A personal recovery key is a unique code that can be used to unlock the user’s device, even if the password to the device is lost.</span></span>|





