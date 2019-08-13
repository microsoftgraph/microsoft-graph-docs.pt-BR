---
title: tipo de enumeração macOSFileVaultRecoveryKeyTypes
description: Tipos de chave de recuperação para macOS FileVault
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1a72cc8ddb4e9ce28a65e3af006ebec097eda247
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365052"
---
# <a name="macosfilevaultrecoverykeytypes-enum-type"></a><span data-ttu-id="6dc10-103">tipo de enumeração macOSFileVaultRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="6dc10-103">macOSFileVaultRecoveryKeyTypes enum type</span></span>

> <span data-ttu-id="6dc10-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6dc10-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6dc10-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6dc10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dc10-106">Tipos de chave de recuperação para macOS FileVault</span><span class="sxs-lookup"><span data-stu-id="6dc10-106">Recovery key types for macOS FileVault</span></span>

## <a name="members"></a><span data-ttu-id="6dc10-107">Membros</span><span class="sxs-lookup"><span data-stu-id="6dc10-107">Members</span></span>
|<span data-ttu-id="6dc10-108">Membro</span><span class="sxs-lookup"><span data-stu-id="6dc10-108">Member</span></span>|<span data-ttu-id="6dc10-109">Valor</span><span class="sxs-lookup"><span data-stu-id="6dc10-109">Value</span></span>|<span data-ttu-id="6dc10-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dc10-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dc10-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6dc10-111">notConfigured</span></span>|<span data-ttu-id="6dc10-112">,0</span><span class="sxs-lookup"><span data-stu-id="6dc10-112">0</span></span>|<span data-ttu-id="6dc10-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="6dc10-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="6dc10-114">institutionalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="6dc10-114">institutionalRecoveryKey</span></span>|<span data-ttu-id="6dc10-115">1</span><span class="sxs-lookup"><span data-stu-id="6dc10-115">1</span></span>|<span data-ttu-id="6dc10-116">Uma chave de recuperação institucional é como uma chave de recuperação "mestra" que pode ser usada para desbloquear qualquer dispositivo cuja senha tenha sido perdida.</span><span class="sxs-lookup"><span data-stu-id="6dc10-116">An institutional recovery key is like a “master” recovery key that can be used to unlock any device whose password has been lost.</span></span>|
|<span data-ttu-id="6dc10-117">personalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="6dc10-117">personalRecoveryKey</span></span>|<span data-ttu-id="6dc10-118">duas</span><span class="sxs-lookup"><span data-stu-id="6dc10-118">2</span></span>|<span data-ttu-id="6dc10-119">Uma chave de recuperação pessoal é um código exclusivo que pode ser usado para desbloquear o dispositivo do usuário, mesmo se a senha do dispositivo for perdida.</span><span class="sxs-lookup"><span data-stu-id="6dc10-119">A personal recovery key is a unique code that can be used to unlock the user’s device, even if the password to the device is lost.</span></span>|



