---
title: tipo de enum androidDeviceOwnerSystemUpdateInstallType
description: Atualizar tipos de sistema para o proprietário de dispositivo Android.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8d7caaa3c79062bba6b8aa06ea11389e1370fba5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419174"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="2ff89-103">tipo de enum androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="2ff89-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

> <span data-ttu-id="2ff89-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="2ff89-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2ff89-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2ff89-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ff89-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="2ff89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ff89-107">Atualizar tipos de sistema para o proprietário de dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="2ff89-107">System Update Types for Android Device Owner.</span></span>

## <a name="members"></a><span data-ttu-id="2ff89-108">Membros</span><span class="sxs-lookup"><span data-stu-id="2ff89-108">Members</span></span>
|<span data-ttu-id="2ff89-109">Membro</span><span class="sxs-lookup"><span data-stu-id="2ff89-109">Member</span></span>|<span data-ttu-id="2ff89-110">Valor</span><span class="sxs-lookup"><span data-stu-id="2ff89-110">Value</span></span>|<span data-ttu-id="2ff89-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ff89-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ff89-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="2ff89-112">deviceDefault</span></span>|<span data-ttu-id="2ff89-113">0</span><span class="sxs-lookup"><span data-stu-id="2ff89-113">0</span></span>|<span data-ttu-id="2ff89-114">Comportamento de padrão de dispositivo, que geralmente solicita que o usuário aceite atualizações de sistema.</span><span class="sxs-lookup"><span data-stu-id="2ff89-114">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="2ff89-115">Adiar</span><span class="sxs-lookup"><span data-stu-id="2ff89-115">postpone</span></span>|<span data-ttu-id="2ff89-116">1</span><span class="sxs-lookup"><span data-stu-id="2ff89-116">1</span></span>|<span data-ttu-id="2ff89-117">Adie a instalação automática das atualizações de backup para 30 dias.</span><span class="sxs-lookup"><span data-stu-id="2ff89-117">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="2ff89-118">em janelas</span><span class="sxs-lookup"><span data-stu-id="2ff89-118">windowed</span></span>|<span data-ttu-id="2ff89-119">2</span><span class="sxs-lookup"><span data-stu-id="2ff89-119">2</span></span>|<span data-ttu-id="2ff89-120">Instale automaticamente dentro de uma janela de manutenção diária.</span><span class="sxs-lookup"><span data-stu-id="2ff89-120">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="2ff89-121">automatic</span><span class="sxs-lookup"><span data-stu-id="2ff89-121">automatic</span></span>|<span data-ttu-id="2ff89-122">3</span><span class="sxs-lookup"><span data-stu-id="2ff89-122">3</span></span>|<span data-ttu-id="2ff89-123">Instale automaticamente atualizações assim que possível.</span><span class="sxs-lookup"><span data-stu-id="2ff89-123">Automatically install updates as soon as possible.</span></span>|




