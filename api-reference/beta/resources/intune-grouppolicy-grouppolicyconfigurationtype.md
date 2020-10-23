---
title: tipo de enumeração groupPolicyConfigurationType
description: Tipo de configuração da política de grupo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 841917ac69bee58ac3559daf9ac4d806a069adda
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697382"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a><span data-ttu-id="9f201-103">tipo de enumeração groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="9f201-103">groupPolicyConfigurationType enum type</span></span>

<span data-ttu-id="9f201-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f201-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f201-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9f201-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f201-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9f201-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f201-107">Tipo de configuração da política de grupo</span><span class="sxs-lookup"><span data-stu-id="9f201-107">Group Policy Configuration Type</span></span>

## <a name="members"></a><span data-ttu-id="9f201-108">Membros</span><span class="sxs-lookup"><span data-stu-id="9f201-108">Members</span></span>
|<span data-ttu-id="9f201-109">Membro</span><span class="sxs-lookup"><span data-stu-id="9f201-109">Member</span></span>|<span data-ttu-id="9f201-110">Valor</span><span class="sxs-lookup"><span data-stu-id="9f201-110">Value</span></span>|<span data-ttu-id="9f201-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f201-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f201-112">política</span><span class="sxs-lookup"><span data-stu-id="9f201-112">policy</span></span>|<span data-ttu-id="9f201-113">,0</span><span class="sxs-lookup"><span data-stu-id="9f201-113">0</span></span>|<span data-ttu-id="9f201-114">O tipo de política não é de Tattoo o valor, o que significa que o valor é removido, permitindo que o valor de configuração original seja usado.</span><span class="sxs-lookup"><span data-stu-id="9f201-114">The policy type does not tattoo the value, which means the value is removed allowing the original configuration value to be used.</span></span> <span data-ttu-id="9f201-115">O tipo de política substitui a definição de configuração de aplicativo para que o aplicativo sempre saiba o valor.</span><span class="sxs-lookup"><span data-stu-id="9f201-115">The policy type supercedes application configuration setting so the application is always aware of the value.</span></span> <span data-ttu-id="9f201-116">O tipo de política impede que o usuário modifique o valor por meio da interface do usuário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9f201-116">The policy type prevents the user from modifying the value through the application's user interface.</span></span>|
|<span data-ttu-id="9f201-117">preferência</span><span class="sxs-lookup"><span data-stu-id="9f201-117">preference</span></span>|<span data-ttu-id="9f201-118">1</span><span class="sxs-lookup"><span data-stu-id="9f201-118">1</span></span>|<span data-ttu-id="9f201-119">O tipo de preferência tem o valor de Tattoo, o que significa que o valor não é removido do registro.</span><span class="sxs-lookup"><span data-stu-id="9f201-119">The preference type does tattoo the value, which means the value is not removed from the registry.</span></span> <span data-ttu-id="9f201-120">O tipo de preferência substituirá o valor configurado pelo usuário e não manterá o valor anterior.</span><span class="sxs-lookup"><span data-stu-id="9f201-120">The preference type will overwrite the user configured-value and does not retain the previous value.</span></span> <span data-ttu-id="9f201-121">O tipo de preferência não impede que o usuário modifique o valor por meio da interface do usuário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9f201-121">The preference type does not prevent the user from modifying the value through the application's user interface.</span></span>|





