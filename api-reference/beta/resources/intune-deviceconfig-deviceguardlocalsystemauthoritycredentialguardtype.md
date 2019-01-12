---
title: tipo de enum deviceGuardLocalSystemAuthorityCredentialGuardType
description: Valores possíveis de configurações do protetor de credencial.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d284b81632c5ba48fa4c658719203a74fdf52837
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952738"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="d8cca-103">tipo de enum deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="d8cca-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="d8cca-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d8cca-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8cca-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d8cca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8cca-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d8cca-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8cca-107">Valores possíveis de configurações do protetor de credencial.</span><span class="sxs-lookup"><span data-stu-id="d8cca-107">Possible values of Credential Guard settings.</span></span>
## <a name="members"></a><span data-ttu-id="d8cca-108">Membros</span><span class="sxs-lookup"><span data-stu-id="d8cca-108">Members</span></span>
|<span data-ttu-id="d8cca-109">Membro</span><span class="sxs-lookup"><span data-stu-id="d8cca-109">Member</span></span>|<span data-ttu-id="d8cca-110">Valor</span><span class="sxs-lookup"><span data-stu-id="d8cca-110">Value</span></span>|<span data-ttu-id="d8cca-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8cca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8cca-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="d8cca-112">notConfigured</span></span>|<span data-ttu-id="d8cca-113">0</span><span class="sxs-lookup"><span data-stu-id="d8cca-113">0</span></span>|<span data-ttu-id="d8cca-114">Desativa a credencial Guard remotamente se configurado anteriormente sem bloqueio UEFI.</span><span class="sxs-lookup"><span data-stu-id="d8cca-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="d8cca-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="d8cca-115">enableWithUEFILock</span></span>|<span data-ttu-id="d8cca-116">1</span><span class="sxs-lookup"><span data-stu-id="d8cca-116">1</span></span>|<span data-ttu-id="d8cca-117">Ativa o protetor de credencial com lock UEFI.</span><span class="sxs-lookup"><span data-stu-id="d8cca-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="d8cca-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="d8cca-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="d8cca-119">2</span><span class="sxs-lookup"><span data-stu-id="d8cca-119">2</span></span>|<span data-ttu-id="d8cca-120">Ativa o protetor de credencial sem bloqueio UEFI.</span><span class="sxs-lookup"><span data-stu-id="d8cca-120">Turns on Credential Guard without UEFI lock.</span></span>|





