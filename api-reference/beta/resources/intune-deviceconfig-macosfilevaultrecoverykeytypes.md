---
title: tipo de enumeração macOSFileVaultRecoveryKeyTypes
description: Tipos de chave de recuperação para macOS FileVault
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 931e04d687590312a015ecc4e6f2e40f0e4dca10
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279945"
---
# <a name="macosfilevaultrecoverykeytypes-enum-type"></a><span data-ttu-id="4b300-103">tipo de enumeração macOSFileVaultRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="4b300-103">macOSFileVaultRecoveryKeyTypes enum type</span></span>

<span data-ttu-id="4b300-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b300-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b300-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4b300-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b300-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4b300-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b300-107">Tipos de chave de recuperação para macOS FileVault</span><span class="sxs-lookup"><span data-stu-id="4b300-107">Recovery key types for macOS FileVault</span></span>

## <a name="members"></a><span data-ttu-id="4b300-108">Membros</span><span class="sxs-lookup"><span data-stu-id="4b300-108">Members</span></span>
|<span data-ttu-id="4b300-109">Membro</span><span class="sxs-lookup"><span data-stu-id="4b300-109">Member</span></span>|<span data-ttu-id="4b300-110">Valor</span><span class="sxs-lookup"><span data-stu-id="4b300-110">Value</span></span>|<span data-ttu-id="4b300-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b300-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b300-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4b300-112">notConfigured</span></span>|<span data-ttu-id="4b300-113">,0</span><span class="sxs-lookup"><span data-stu-id="4b300-113">0</span></span>|<span data-ttu-id="4b300-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="4b300-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="4b300-115">institutionalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="4b300-115">institutionalRecoveryKey</span></span>|<span data-ttu-id="4b300-116">1</span><span class="sxs-lookup"><span data-stu-id="4b300-116">1</span></span>|<span data-ttu-id="4b300-117">Uma chave de recuperação institucional é como uma chave de recuperação "mestra" que pode ser usada para desbloquear qualquer dispositivo cuja senha tenha sido perdida.</span><span class="sxs-lookup"><span data-stu-id="4b300-117">An institutional recovery key is like a “master” recovery key that can be used to unlock any device whose password has been lost.</span></span>|
|<span data-ttu-id="4b300-118">personalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="4b300-118">personalRecoveryKey</span></span>|<span data-ttu-id="4b300-119">duas</span><span class="sxs-lookup"><span data-stu-id="4b300-119">2</span></span>|<span data-ttu-id="4b300-120">Uma chave de recuperação pessoal é um código exclusivo que pode ser usado para desbloquear o dispositivo do usuário, mesmo se a senha do dispositivo for perdida.</span><span class="sxs-lookup"><span data-stu-id="4b300-120">A personal recovery key is a unique code that can be used to unlock the user’s device, even if the password to the device is lost.</span></span>|




