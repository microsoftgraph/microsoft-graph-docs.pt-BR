---
title: tipo de enum roleAssignmentScopeType
description: Especifica o tipo de escopo para uma atribuição de função.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b72e74bdb401f556214470b4c0aeda651339e332
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916079"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="d3ce4-103">tipo de enum roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="d3ce4-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="d3ce4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d3ce4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3ce4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d3ce4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d3ce4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d3ce4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3ce4-107">Especifica o tipo de escopo para uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d3ce4-107">Specifies the type of scope for a Role Assignment.</span></span>
## <a name="members"></a><span data-ttu-id="d3ce4-108">Membros</span><span class="sxs-lookup"><span data-stu-id="d3ce4-108">Members</span></span>
|<span data-ttu-id="d3ce4-109">Membro</span><span class="sxs-lookup"><span data-stu-id="d3ce4-109">Member</span></span>|<span data-ttu-id="d3ce4-110">Valor</span><span class="sxs-lookup"><span data-stu-id="d3ce4-110">Value</span></span>|<span data-ttu-id="d3ce4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3ce4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3ce4-112">resourceScope</span><span class="sxs-lookup"><span data-stu-id="d3ce4-112">resourceScope</span></span>|<span data-ttu-id="d3ce4-113">0</span><span class="sxs-lookup"><span data-stu-id="d3ce4-113">0</span></span>|<span data-ttu-id="d3ce4-114">Permitir que as atribuições para o ResourceScopes especificado.</span><span class="sxs-lookup"><span data-stu-id="d3ce4-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="d3ce4-115">allDevices</span><span class="sxs-lookup"><span data-stu-id="d3ce4-115">allDevices</span></span>|<span data-ttu-id="d3ce4-116">1</span><span class="sxs-lookup"><span data-stu-id="d3ce4-116">1</span></span>|<span data-ttu-id="d3ce4-117">Permitir que as atribuições para todos os dispositivos Intune.</span><span class="sxs-lookup"><span data-stu-id="d3ce4-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="d3ce4-118">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="d3ce4-118">allLicensedUsers</span></span>|<span data-ttu-id="d3ce4-119">2</span><span class="sxs-lookup"><span data-stu-id="d3ce4-119">2</span></span>|<span data-ttu-id="d3ce4-120">Permitir que as atribuições para todos os usuários licenciado do Intune.</span><span class="sxs-lookup"><span data-stu-id="d3ce4-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="d3ce4-121">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="d3ce4-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="d3ce4-122">3</span><span class="sxs-lookup"><span data-stu-id="d3ce4-122">3</span></span>|<span data-ttu-id="d3ce4-123">Permitir que as atribuições para todos os dispositivos de Intune e os usuários licenciados.</span><span class="sxs-lookup"><span data-stu-id="d3ce4-123">Allow assignments to all Intune devices and licensed users.</span></span>|





