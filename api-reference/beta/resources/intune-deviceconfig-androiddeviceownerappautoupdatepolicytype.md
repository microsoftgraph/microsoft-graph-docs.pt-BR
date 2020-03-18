---
title: tipo de enumeração androidDeviceOwnerAppAutoUpdatePolicyType
description: Proprietário do dispositivo Android valores possíveis para Estados da política de atualização automática do aplicativo do dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 55092376dcf0d5e4ae72b5cb6f607cf984959c4d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797175"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="bd11d-103">tipo de enumeração androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="bd11d-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="bd11d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bd11d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd11d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bd11d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd11d-106">Proprietário do dispositivo Android valores possíveis para Estados da política de atualização automática do aplicativo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bd11d-106">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="bd11d-107">Membros</span><span class="sxs-lookup"><span data-stu-id="bd11d-107">Members</span></span>
|<span data-ttu-id="bd11d-108">Membro</span><span class="sxs-lookup"><span data-stu-id="bd11d-108">Member</span></span>|<span data-ttu-id="bd11d-109">Valor</span><span class="sxs-lookup"><span data-stu-id="bd11d-109">Value</span></span>|<span data-ttu-id="bd11d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd11d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd11d-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="bd11d-111">notConfigured</span></span>|<span data-ttu-id="bd11d-112">,0</span><span class="sxs-lookup"><span data-stu-id="bd11d-112">0</span></span>|<span data-ttu-id="bd11d-113">Não configurado; Esse valor é ignorado.</span><span class="sxs-lookup"><span data-stu-id="bd11d-113">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="bd11d-114">UserChoice</span><span class="sxs-lookup"><span data-stu-id="bd11d-114">userChoice</span></span>|<span data-ttu-id="bd11d-115">1</span><span class="sxs-lookup"><span data-stu-id="bd11d-115">1</span></span>|<span data-ttu-id="bd11d-116">O usuário pode controlar as atualizações automáticas.</span><span class="sxs-lookup"><span data-stu-id="bd11d-116">The user can control auto-updates.</span></span>|
|<span data-ttu-id="bd11d-117">Édito</span><span class="sxs-lookup"><span data-stu-id="bd11d-117">never</span></span>|<span data-ttu-id="bd11d-118">duas</span><span class="sxs-lookup"><span data-stu-id="bd11d-118">2</span></span>|<span data-ttu-id="bd11d-119">Os aplicativos nunca são atualizados automaticamente.</span><span class="sxs-lookup"><span data-stu-id="bd11d-119">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="bd11d-120">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="bd11d-120">wiFiOnly</span></span>|<span data-ttu-id="bd11d-121">3D</span><span class="sxs-lookup"><span data-stu-id="bd11d-121">3</span></span>|<span data-ttu-id="bd11d-122">Os aplicativos são atualizados automaticamente através de Wi-Fi apenas.</span><span class="sxs-lookup"><span data-stu-id="bd11d-122">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="bd11d-123">permanente</span><span class="sxs-lookup"><span data-stu-id="bd11d-123">always</span></span>|<span data-ttu-id="bd11d-124">4 </span><span class="sxs-lookup"><span data-stu-id="bd11d-124">4</span></span>|<span data-ttu-id="bd11d-125">Os aplicativos são atualizados automaticamente a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="bd11d-125">Apps are auto-updated at any time.</span></span> <span data-ttu-id="bd11d-126">Tarifas de dados podem ser aplicadas.</span><span class="sxs-lookup"><span data-stu-id="bd11d-126">Data charges may apply.</span></span>|



