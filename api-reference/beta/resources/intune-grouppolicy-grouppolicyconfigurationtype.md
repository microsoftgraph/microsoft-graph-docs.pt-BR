---
title: tipo de enumeração groupPolicyConfigurationType
description: Tipo de configuração da política de grupo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 882544846ea5f714c160ee432e82bbc05e13da51
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031029"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a><span data-ttu-id="85361-103">tipo de enumeração groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="85361-103">groupPolicyConfigurationType enum type</span></span>

<span data-ttu-id="85361-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85361-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85361-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="85361-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85361-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="85361-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85361-107">Tipo de configuração da política de grupo</span><span class="sxs-lookup"><span data-stu-id="85361-107">Group Policy Configuration Type</span></span>

## <a name="members"></a><span data-ttu-id="85361-108">Membros</span><span class="sxs-lookup"><span data-stu-id="85361-108">Members</span></span>
|<span data-ttu-id="85361-109">Membro</span><span class="sxs-lookup"><span data-stu-id="85361-109">Member</span></span>|<span data-ttu-id="85361-110">Valor</span><span class="sxs-lookup"><span data-stu-id="85361-110">Value</span></span>|<span data-ttu-id="85361-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="85361-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85361-112">política</span><span class="sxs-lookup"><span data-stu-id="85361-112">policy</span></span>|<span data-ttu-id="85361-113">,0</span><span class="sxs-lookup"><span data-stu-id="85361-113">0</span></span>|<span data-ttu-id="85361-114">O tipo de política não é de Tattoo o valor, o que significa que o valor é removido, permitindo que o valor de configuração original seja usado.</span><span class="sxs-lookup"><span data-stu-id="85361-114">The policy type does not tattoo the value, which means the value is removed allowing the original configuration value to be used.</span></span> <span data-ttu-id="85361-115">O tipo de política substitui a definição de configuração de aplicativo para que o aplicativo sempre saiba o valor.</span><span class="sxs-lookup"><span data-stu-id="85361-115">The policy type supercedes application configuration setting so the application is always aware of the value.</span></span> <span data-ttu-id="85361-116">O tipo de política impede que o usuário modifique o valor por meio da interface do usuário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="85361-116">The policy type prevents the user from modifying the value through the application's user interface.</span></span>|
|<span data-ttu-id="85361-117">preferência</span><span class="sxs-lookup"><span data-stu-id="85361-117">preference</span></span>|<span data-ttu-id="85361-118">1 </span><span class="sxs-lookup"><span data-stu-id="85361-118">1</span></span>|<span data-ttu-id="85361-119">O tipo de preferência tem o valor de Tattoo, o que significa que o valor não é removido do registro.</span><span class="sxs-lookup"><span data-stu-id="85361-119">The preference type does tattoo the value, which means the value is not removed from the registry.</span></span> <span data-ttu-id="85361-120">O tipo de preferência substituirá o valor configurado pelo usuário e não manterá o valor anterior.</span><span class="sxs-lookup"><span data-stu-id="85361-120">The preference type will overwrite the user configured-value and does not retain the previous value.</span></span> <span data-ttu-id="85361-121">O tipo de preferência não impede que o usuário modifique o valor por meio da interface do usuário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="85361-121">The preference type does not prevent the user from modifying the value through the application's user interface.</span></span>|






