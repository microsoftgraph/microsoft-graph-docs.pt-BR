---
title: tipo de enumeração androidDeviceOwnerAppAutoUpdatePolicyType
description: Proprietário do dispositivo Android valores possíveis para Estados da política de atualização automática do aplicativo do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5460053da38a09fdc4df4de0b4030b9081c19d0d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076103"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="60feb-103">tipo de enumeração androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="60feb-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

<span data-ttu-id="60feb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60feb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60feb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="60feb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60feb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="60feb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60feb-107">Proprietário do dispositivo Android valores possíveis para Estados da política de atualização automática do aplicativo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="60feb-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="60feb-108">Membros</span><span class="sxs-lookup"><span data-stu-id="60feb-108">Members</span></span>
|<span data-ttu-id="60feb-109">Membro</span><span class="sxs-lookup"><span data-stu-id="60feb-109">Member</span></span>|<span data-ttu-id="60feb-110">Valor</span><span class="sxs-lookup"><span data-stu-id="60feb-110">Value</span></span>|<span data-ttu-id="60feb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="60feb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60feb-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="60feb-112">notConfigured</span></span>|<span data-ttu-id="60feb-113">,0</span><span class="sxs-lookup"><span data-stu-id="60feb-113">0</span></span>|<span data-ttu-id="60feb-114">Não configurado; Esse valor é ignorado.</span><span class="sxs-lookup"><span data-stu-id="60feb-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="60feb-115">UserChoice</span><span class="sxs-lookup"><span data-stu-id="60feb-115">userChoice</span></span>|<span data-ttu-id="60feb-116">1 </span><span class="sxs-lookup"><span data-stu-id="60feb-116">1</span></span>|<span data-ttu-id="60feb-117">O usuário pode controlar as atualizações automáticas.</span><span class="sxs-lookup"><span data-stu-id="60feb-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="60feb-118">Édito</span><span class="sxs-lookup"><span data-stu-id="60feb-118">never</span></span>|<span data-ttu-id="60feb-119">2 </span><span class="sxs-lookup"><span data-stu-id="60feb-119">2</span></span>|<span data-ttu-id="60feb-120">Os aplicativos nunca são atualizados automaticamente.</span><span class="sxs-lookup"><span data-stu-id="60feb-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="60feb-121">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="60feb-121">wiFiOnly</span></span>|<span data-ttu-id="60feb-122">3 </span><span class="sxs-lookup"><span data-stu-id="60feb-122">3</span></span>|<span data-ttu-id="60feb-123">Os aplicativos são atualizados automaticamente através de Wi-Fi apenas.</span><span class="sxs-lookup"><span data-stu-id="60feb-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="60feb-124">permanente</span><span class="sxs-lookup"><span data-stu-id="60feb-124">always</span></span>|<span data-ttu-id="60feb-125">4 </span><span class="sxs-lookup"><span data-stu-id="60feb-125">4</span></span>|<span data-ttu-id="60feb-126">Os aplicativos são atualizados automaticamente a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="60feb-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="60feb-127">Tarifas de dados podem ser aplicadas.</span><span class="sxs-lookup"><span data-stu-id="60feb-127">Data charges may apply.</span></span>|






