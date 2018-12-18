---
title: tipo de enum androidDeviceOwnerSystemUpdateInstallType
description: Atualizar tipos de sistema para o proprietário de dispositivo Android.
author: tfitzmac
ms.openlocfilehash: e2dc66851e0fa98d52a3fec30385e0fd27e6f6ca
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323195"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="183f0-103">tipo de enum androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="183f0-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

> <span data-ttu-id="183f0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="183f0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="183f0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="183f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="183f0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="183f0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="183f0-107">Atualizar tipos de sistema para o proprietário de dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="183f0-107">System Update Types for Android Device Owner.</span></span>
## <a name="members"></a><span data-ttu-id="183f0-108">Membros</span><span class="sxs-lookup"><span data-stu-id="183f0-108">Members</span></span>
|<span data-ttu-id="183f0-109">Membro</span><span class="sxs-lookup"><span data-stu-id="183f0-109">Member</span></span>|<span data-ttu-id="183f0-110">Valor</span><span class="sxs-lookup"><span data-stu-id="183f0-110">Value</span></span>|<span data-ttu-id="183f0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="183f0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="183f0-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="183f0-112">deviceDefault</span></span>|<span data-ttu-id="183f0-113">0</span><span class="sxs-lookup"><span data-stu-id="183f0-113">0</span></span>|<span data-ttu-id="183f0-114">Comportamento de padrão de dispositivo, que geralmente solicita que o usuário aceite atualizações de sistema.</span><span class="sxs-lookup"><span data-stu-id="183f0-114">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="183f0-115">Adiar</span><span class="sxs-lookup"><span data-stu-id="183f0-115">postpone</span></span>|<span data-ttu-id="183f0-116">1</span><span class="sxs-lookup"><span data-stu-id="183f0-116">1</span></span>|<span data-ttu-id="183f0-117">Adie a instalação automática das atualizações de backup para 30 dias.</span><span class="sxs-lookup"><span data-stu-id="183f0-117">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="183f0-118">em janelas</span><span class="sxs-lookup"><span data-stu-id="183f0-118">windowed</span></span>|<span data-ttu-id="183f0-119">2</span><span class="sxs-lookup"><span data-stu-id="183f0-119">2</span></span>|<span data-ttu-id="183f0-120">Instale automaticamente dentro de uma janela de manutenção diária.</span><span class="sxs-lookup"><span data-stu-id="183f0-120">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="183f0-121">automatic</span><span class="sxs-lookup"><span data-stu-id="183f0-121">automatic</span></span>|<span data-ttu-id="183f0-122">3</span><span class="sxs-lookup"><span data-stu-id="183f0-122">3</span></span>|<span data-ttu-id="183f0-123">Instale automaticamente atualizações assim que possível.</span><span class="sxs-lookup"><span data-stu-id="183f0-123">Automatically install updates as soon as possible.</span></span>|





