---
title: tipo de enumeração groupPolicyConfigurationType
description: Tipo de configuração da política de grupo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c0d3a0daa73fef30e5425e188958bdc54e61778d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164684"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a><span data-ttu-id="8be87-103">tipo de enumeração groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="8be87-103">groupPolicyConfigurationType enum type</span></span>

> <span data-ttu-id="8be87-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8be87-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8be87-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8be87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8be87-106">Tipo de configuração da política de grupo</span><span class="sxs-lookup"><span data-stu-id="8be87-106">Group Policy Configuration Type</span></span>

## <a name="members"></a><span data-ttu-id="8be87-107">Membros</span><span class="sxs-lookup"><span data-stu-id="8be87-107">Members</span></span>
|<span data-ttu-id="8be87-108">Membro</span><span class="sxs-lookup"><span data-stu-id="8be87-108">Member</span></span>|<span data-ttu-id="8be87-109">Valor</span><span class="sxs-lookup"><span data-stu-id="8be87-109">Value</span></span>|<span data-ttu-id="8be87-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8be87-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8be87-111">política</span><span class="sxs-lookup"><span data-stu-id="8be87-111">policy</span></span>|<span data-ttu-id="8be87-112">,0</span><span class="sxs-lookup"><span data-stu-id="8be87-112">0</span></span>|<span data-ttu-id="8be87-113">O tipo de política não é de Tattoo o valor, o que significa que o valor é removido, permitindo que o valor de configuração original seja usado.</span><span class="sxs-lookup"><span data-stu-id="8be87-113">The policy type does not tattoo the value, which means the value is removed allowing the original configuration value to be used.</span></span> <span data-ttu-id="8be87-114">O tipo de política substitui a definição de configuração de aplicativo para que o aplicativo sempre saiba o valor.</span><span class="sxs-lookup"><span data-stu-id="8be87-114">The policy type supercedes application configuration setting so the application is always aware of the value.</span></span> <span data-ttu-id="8be87-115">O tipo de política impede que o usuário modifique o valor por meio da interface do usuário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8be87-115">The policy type prevents the user from modifying the value through the application's user interface.</span></span>|
|<span data-ttu-id="8be87-116">preference</span><span class="sxs-lookup"><span data-stu-id="8be87-116">preference</span></span>|<span data-ttu-id="8be87-117">1</span><span class="sxs-lookup"><span data-stu-id="8be87-117">1</span></span>|<span data-ttu-id="8be87-118">O tipo de preferência tem o valor de Tattoo, o que significa que o valor não é removido do registro.</span><span class="sxs-lookup"><span data-stu-id="8be87-118">The preference type does tattoo the value, which means the value is not removed from the registry.</span></span> <span data-ttu-id="8be87-119">O tipo de preferência substituirá o valor configurado pelo usuário e não manterá o valor anterior.</span><span class="sxs-lookup"><span data-stu-id="8be87-119">The preference type will overwrite the user configured-value and does not retain the previous value.</span></span> <span data-ttu-id="8be87-120">O tipo de preferência não impede que o usuário modifique o valor por meio da interface do usuário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8be87-120">The preference type does not prevent the user from modifying the value through the application's user interface.</span></span>|




