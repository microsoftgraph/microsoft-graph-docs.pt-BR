---
title: tipo de enumeração androidDeviceOwnerAppAutoUpdatePolicyType
description: Proprietário do dispositivo Android valores possíveis para Estados da política de atualização automática do aplicativo do dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 703e8bbb46ae289acfa09267052f9c78fe0da912
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34965715"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="03530-103">tipo de enumeração androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="03530-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="03530-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="03530-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03530-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="03530-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03530-106">Proprietário do dispositivo Android valores possíveis para Estados da política de atualização automática do aplicativo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03530-106">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="03530-107">Membros</span><span class="sxs-lookup"><span data-stu-id="03530-107">Members</span></span>
|<span data-ttu-id="03530-108">Membro</span><span class="sxs-lookup"><span data-stu-id="03530-108">Member</span></span>|<span data-ttu-id="03530-109">Valor</span><span class="sxs-lookup"><span data-stu-id="03530-109">Value</span></span>|<span data-ttu-id="03530-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="03530-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03530-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="03530-111">notConfigured</span></span>|<span data-ttu-id="03530-112">,0</span><span class="sxs-lookup"><span data-stu-id="03530-112">0</span></span>|<span data-ttu-id="03530-113">Não configurado; Esse valor é ignorado.</span><span class="sxs-lookup"><span data-stu-id="03530-113">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="03530-114">UserChoice</span><span class="sxs-lookup"><span data-stu-id="03530-114">userChoice</span></span>|<span data-ttu-id="03530-115">1</span><span class="sxs-lookup"><span data-stu-id="03530-115">1</span></span>|<span data-ttu-id="03530-116">O usuário pode controlar as atualizações automáticas.</span><span class="sxs-lookup"><span data-stu-id="03530-116">The user can control auto-updates.</span></span>|
|<span data-ttu-id="03530-117">Édito</span><span class="sxs-lookup"><span data-stu-id="03530-117">never</span></span>|<span data-ttu-id="03530-118">duas</span><span class="sxs-lookup"><span data-stu-id="03530-118">2</span></span>|<span data-ttu-id="03530-119">Os aplicativos nunca são atualizados automaticamente.</span><span class="sxs-lookup"><span data-stu-id="03530-119">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="03530-120">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="03530-120">wiFiOnly</span></span>|<span data-ttu-id="03530-121">3D</span><span class="sxs-lookup"><span data-stu-id="03530-121">3</span></span>|<span data-ttu-id="03530-122">Os aplicativos são atualizados automaticamente através de Wi-Fi apenas.</span><span class="sxs-lookup"><span data-stu-id="03530-122">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="03530-123">permanente</span><span class="sxs-lookup"><span data-stu-id="03530-123">always</span></span>|<span data-ttu-id="03530-124">quatro</span><span class="sxs-lookup"><span data-stu-id="03530-124">4</span></span>|<span data-ttu-id="03530-125">Os aplicativos são atualizados automaticamente a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="03530-125">Apps are auto-updated at any time.</span></span> <span data-ttu-id="03530-126">Tarifas de dados podem ser aplicadas.</span><span class="sxs-lookup"><span data-stu-id="03530-126">Data charges may apply.</span></span>|





