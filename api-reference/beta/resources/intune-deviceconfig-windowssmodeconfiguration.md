---
title: tipo de enum windowsSModeConfiguration
description: As possíveis opções para configurar o modo S desbloquear
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9e37bd51be1b5476e8b4590b92b3caeeed92ac45
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830734"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="09a03-103">tipo de enum windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="09a03-103">windowsSModeConfiguration enum type</span></span>

> <span data-ttu-id="09a03-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="09a03-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09a03-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="09a03-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09a03-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="09a03-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09a03-107">As possíveis opções para configurar o modo S desbloquear</span><span class="sxs-lookup"><span data-stu-id="09a03-107">The possible options to configure S mode unlock</span></span>
## <a name="members"></a><span data-ttu-id="09a03-108">Membros</span><span class="sxs-lookup"><span data-stu-id="09a03-108">Members</span></span>
|<span data-ttu-id="09a03-109">Membro</span><span class="sxs-lookup"><span data-stu-id="09a03-109">Member</span></span>|<span data-ttu-id="09a03-110">Valor</span><span class="sxs-lookup"><span data-stu-id="09a03-110">Value</span></span>|<span data-ttu-id="09a03-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="09a03-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09a03-112">noRestriction</span><span class="sxs-lookup"><span data-stu-id="09a03-112">noRestriction</span></span>|<span data-ttu-id="09a03-113">0</span><span class="sxs-lookup"><span data-stu-id="09a03-113">0</span></span>|<span data-ttu-id="09a03-114">Essa opção removerá todas as restrições para desbloquear o modo S - padrão</span><span class="sxs-lookup"><span data-stu-id="09a03-114">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="09a03-115">bloquear</span><span class="sxs-lookup"><span data-stu-id="09a03-115">block</span></span>|<span data-ttu-id="09a03-116">1</span><span class="sxs-lookup"><span data-stu-id="09a03-116">1</span></span>|<span data-ttu-id="09a03-117">Essa opção bloqueia o usuário para desbloquear o dispositivo de modo S</span><span class="sxs-lookup"><span data-stu-id="09a03-117">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="09a03-118">desbloquear</span><span class="sxs-lookup"><span data-stu-id="09a03-118">unlock</span></span>|<span data-ttu-id="09a03-119">2</span><span class="sxs-lookup"><span data-stu-id="09a03-119">2</span></span>|<span data-ttu-id="09a03-120">Essa opção será desbloquear o dispositivo de modo S</span><span class="sxs-lookup"><span data-stu-id="09a03-120">This option will unlock the device from S mode</span></span>|





