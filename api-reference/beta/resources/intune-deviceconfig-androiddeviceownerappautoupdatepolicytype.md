---
title: tipo de enum androidDeviceOwnerAppAutoUpdatePolicyType
description: Os valores possíveis proprietário do dispositivo Android para estados da automático do aplicativo do dispositivo atualizam a política.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: f784e951df2a9d1ee56825649da3899b0792c3a6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973605"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="8f086-103">tipo de enum androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="8f086-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="8f086-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8f086-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f086-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8f086-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f086-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8f086-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f086-107">Os valores possíveis proprietário do dispositivo Android para estados da automático do aplicativo do dispositivo atualizam a política.</span><span class="sxs-lookup"><span data-stu-id="8f086-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>
## <a name="members"></a><span data-ttu-id="8f086-108">Membros</span><span class="sxs-lookup"><span data-stu-id="8f086-108">Members</span></span>
|<span data-ttu-id="8f086-109">Membro</span><span class="sxs-lookup"><span data-stu-id="8f086-109">Member</span></span>|<span data-ttu-id="8f086-110">Valor</span><span class="sxs-lookup"><span data-stu-id="8f086-110">Value</span></span>|<span data-ttu-id="8f086-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f086-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f086-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="8f086-112">notConfigured</span></span>|<span data-ttu-id="8f086-113">0</span><span class="sxs-lookup"><span data-stu-id="8f086-113">0</span></span>|<span data-ttu-id="8f086-114">Não configurado; Este valor será ignorado.</span><span class="sxs-lookup"><span data-stu-id="8f086-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="8f086-115">userChoice</span><span class="sxs-lookup"><span data-stu-id="8f086-115">userChoice</span></span>|<span data-ttu-id="8f086-116">1</span><span class="sxs-lookup"><span data-stu-id="8f086-116">1</span></span>|<span data-ttu-id="8f086-117">O usuário pode controlar atualizações automáticas.</span><span class="sxs-lookup"><span data-stu-id="8f086-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="8f086-118">nunca</span><span class="sxs-lookup"><span data-stu-id="8f086-118">never</span></span>|<span data-ttu-id="8f086-119">2</span><span class="sxs-lookup"><span data-stu-id="8f086-119">2</span></span>|<span data-ttu-id="8f086-120">Aplicativos nunca são atualizados para automático.</span><span class="sxs-lookup"><span data-stu-id="8f086-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="8f086-121">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="8f086-121">wiFiOnly</span></span>|<span data-ttu-id="8f086-122">3</span><span class="sxs-lookup"><span data-stu-id="8f086-122">3</span></span>|<span data-ttu-id="8f086-123">Aplicativos atualizado automaticamente por Wi-Fi só estarão.</span><span class="sxs-lookup"><span data-stu-id="8f086-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="8f086-124">sempre</span><span class="sxs-lookup"><span data-stu-id="8f086-124">always</span></span>|<span data-ttu-id="8f086-125">4</span><span class="sxs-lookup"><span data-stu-id="8f086-125">4</span></span>|<span data-ttu-id="8f086-126">Aplicativos são atualizado automaticamente a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="8f086-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="8f086-127">Tarifas de dados podem ser aplicadas.</span><span class="sxs-lookup"><span data-stu-id="8f086-127">Data charges may apply.</span></span>|





