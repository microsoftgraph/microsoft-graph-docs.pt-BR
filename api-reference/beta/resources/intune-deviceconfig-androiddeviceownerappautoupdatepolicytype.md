---
title: tipo de enumeração androidDeviceOwnerAppAutoUpdatePolicyType
description: Proprietário do dispositivo Android valores possíveis para Estados da política de atualização automática do aplicativo do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f7eb22977f571d0e15e8d9cd20f3ee02e52faff7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49216735"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="f46a0-103">tipo de enumeração androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="f46a0-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

<span data-ttu-id="f46a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f46a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f46a0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f46a0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f46a0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f46a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f46a0-107">Proprietário do dispositivo Android valores possíveis para Estados da política de atualização automática do aplicativo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f46a0-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="f46a0-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f46a0-108">Members</span></span>
|<span data-ttu-id="f46a0-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f46a0-109">Member</span></span>|<span data-ttu-id="f46a0-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f46a0-110">Value</span></span>|<span data-ttu-id="f46a0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f46a0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f46a0-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f46a0-112">notConfigured</span></span>|<span data-ttu-id="f46a0-113">,0</span><span class="sxs-lookup"><span data-stu-id="f46a0-113">0</span></span>|<span data-ttu-id="f46a0-114">Não configurado; Esse valor é ignorado.</span><span class="sxs-lookup"><span data-stu-id="f46a0-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="f46a0-115">UserChoice</span><span class="sxs-lookup"><span data-stu-id="f46a0-115">userChoice</span></span>|<span data-ttu-id="f46a0-116">1</span><span class="sxs-lookup"><span data-stu-id="f46a0-116">1</span></span>|<span data-ttu-id="f46a0-117">O usuário pode controlar as atualizações automáticas.</span><span class="sxs-lookup"><span data-stu-id="f46a0-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="f46a0-118">Édito</span><span class="sxs-lookup"><span data-stu-id="f46a0-118">never</span></span>|<span data-ttu-id="f46a0-119">duas</span><span class="sxs-lookup"><span data-stu-id="f46a0-119">2</span></span>|<span data-ttu-id="f46a0-120">Os aplicativos nunca são atualizados automaticamente.</span><span class="sxs-lookup"><span data-stu-id="f46a0-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="f46a0-121">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="f46a0-121">wiFiOnly</span></span>|<span data-ttu-id="f46a0-122">3D</span><span class="sxs-lookup"><span data-stu-id="f46a0-122">3</span></span>|<span data-ttu-id="f46a0-123">Os aplicativos são atualizados automaticamente através do Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f46a0-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="f46a0-124">permanente</span><span class="sxs-lookup"><span data-stu-id="f46a0-124">always</span></span>|<span data-ttu-id="f46a0-125">4 </span><span class="sxs-lookup"><span data-stu-id="f46a0-125">4</span></span>|<span data-ttu-id="f46a0-126">Os aplicativos são atualizados automaticamente a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="f46a0-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="f46a0-127">Tarifas de dados podem ser aplicadas.</span><span class="sxs-lookup"><span data-stu-id="f46a0-127">Data charges may apply.</span></span>|




