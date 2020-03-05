---
title: tipo de enumeração androidDeviceOwnerAppAutoUpdatePolicyType
description: Proprietário do dispositivo Android valores possíveis para Estados da política de atualização automática do aplicativo do dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: cd003c8213faf45453f1b6165931181250c861ec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42487197"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="60c13-103">tipo de enumeração androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="60c13-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

<span data-ttu-id="60c13-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="60c13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60c13-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="60c13-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60c13-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="60c13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60c13-107">Proprietário do dispositivo Android valores possíveis para Estados da política de atualização automática do aplicativo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="60c13-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="60c13-108">Membros</span><span class="sxs-lookup"><span data-stu-id="60c13-108">Members</span></span>
|<span data-ttu-id="60c13-109">Membro</span><span class="sxs-lookup"><span data-stu-id="60c13-109">Member</span></span>|<span data-ttu-id="60c13-110">Valor</span><span class="sxs-lookup"><span data-stu-id="60c13-110">Value</span></span>|<span data-ttu-id="60c13-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="60c13-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60c13-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="60c13-112">notConfigured</span></span>|<span data-ttu-id="60c13-113">,0</span><span class="sxs-lookup"><span data-stu-id="60c13-113">0</span></span>|<span data-ttu-id="60c13-114">Não configurado; Esse valor é ignorado.</span><span class="sxs-lookup"><span data-stu-id="60c13-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="60c13-115">UserChoice</span><span class="sxs-lookup"><span data-stu-id="60c13-115">userChoice</span></span>|<span data-ttu-id="60c13-116">1 </span><span class="sxs-lookup"><span data-stu-id="60c13-116">1</span></span>|<span data-ttu-id="60c13-117">O usuário pode controlar as atualizações automáticas.</span><span class="sxs-lookup"><span data-stu-id="60c13-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="60c13-118">Édito</span><span class="sxs-lookup"><span data-stu-id="60c13-118">never</span></span>|<span data-ttu-id="60c13-119">2 </span><span class="sxs-lookup"><span data-stu-id="60c13-119">2</span></span>|<span data-ttu-id="60c13-120">Os aplicativos nunca são atualizados automaticamente.</span><span class="sxs-lookup"><span data-stu-id="60c13-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="60c13-121">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="60c13-121">wiFiOnly</span></span>|<span data-ttu-id="60c13-122">3 </span><span class="sxs-lookup"><span data-stu-id="60c13-122">3</span></span>|<span data-ttu-id="60c13-123">Os aplicativos são atualizados automaticamente através de Wi-Fi apenas.</span><span class="sxs-lookup"><span data-stu-id="60c13-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="60c13-124">permanente</span><span class="sxs-lookup"><span data-stu-id="60c13-124">always</span></span>|<span data-ttu-id="60c13-125">4 </span><span class="sxs-lookup"><span data-stu-id="60c13-125">4</span></span>|<span data-ttu-id="60c13-126">Os aplicativos são atualizados automaticamente a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="60c13-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="60c13-127">Tarifas de dados podem ser aplicadas.</span><span class="sxs-lookup"><span data-stu-id="60c13-127">Data charges may apply.</span></span>|



