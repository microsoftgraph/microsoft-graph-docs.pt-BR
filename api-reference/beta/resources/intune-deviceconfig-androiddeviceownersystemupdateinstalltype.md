---
title: tipo de enumeração androidDeviceOwnerSystemUpdateInstallType
description: Tipos de atualização do sistema para o proprietário do dispositivo Android.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b64de74146e6ee6ffe30416d03277919e06490d2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43402770"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="55ad0-103">tipo de enumeração androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="55ad0-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

<span data-ttu-id="55ad0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55ad0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55ad0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="55ad0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55ad0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55ad0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55ad0-107">Tipos de atualização do sistema para o proprietário do dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="55ad0-107">System Update Types for Android Device Owner.</span></span>

## <a name="members"></a><span data-ttu-id="55ad0-108">Membros</span><span class="sxs-lookup"><span data-stu-id="55ad0-108">Members</span></span>
|<span data-ttu-id="55ad0-109">Membro</span><span class="sxs-lookup"><span data-stu-id="55ad0-109">Member</span></span>|<span data-ttu-id="55ad0-110">Valor</span><span class="sxs-lookup"><span data-stu-id="55ad0-110">Value</span></span>|<span data-ttu-id="55ad0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="55ad0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55ad0-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="55ad0-112">deviceDefault</span></span>|<span data-ttu-id="55ad0-113">,0</span><span class="sxs-lookup"><span data-stu-id="55ad0-113">0</span></span>|<span data-ttu-id="55ad0-114">Comportamento padrão do dispositivo, que normalmente solicita que o usuário aceite atualizações do sistema.</span><span class="sxs-lookup"><span data-stu-id="55ad0-114">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="55ad0-115">adiamento</span><span class="sxs-lookup"><span data-stu-id="55ad0-115">postpone</span></span>|<span data-ttu-id="55ad0-116">1</span><span class="sxs-lookup"><span data-stu-id="55ad0-116">1</span></span>|<span data-ttu-id="55ad0-117">Adiar a instalação automática de atualizações até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="55ad0-117">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="55ad0-118">em janelas</span><span class="sxs-lookup"><span data-stu-id="55ad0-118">windowed</span></span>|<span data-ttu-id="55ad0-119">duas</span><span class="sxs-lookup"><span data-stu-id="55ad0-119">2</span></span>|<span data-ttu-id="55ad0-120">Instale automaticamente dentro de uma janela de manutenção diária.</span><span class="sxs-lookup"><span data-stu-id="55ad0-120">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="55ad0-121">Automático</span><span class="sxs-lookup"><span data-stu-id="55ad0-121">automatic</span></span>|<span data-ttu-id="55ad0-122">3D</span><span class="sxs-lookup"><span data-stu-id="55ad0-122">3</span></span>|<span data-ttu-id="55ad0-123">Instalar atualizações automaticamente o mais rápido possível.</span><span class="sxs-lookup"><span data-stu-id="55ad0-123">Automatically install updates as soon as possible.</span></span>|



