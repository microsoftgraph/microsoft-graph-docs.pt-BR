---
title: tipo de enumeração roleAssignmentScopeType
description: Especifica o tipo de escopo de uma atribuição de função.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f922cf51729f178ab9ca94db127efb5b70bb94fe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523890"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="61b4a-103">tipo de enumeração roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="61b4a-103">roleAssignmentScopeType enum type</span></span>

<span data-ttu-id="61b4a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="61b4a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61b4a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="61b4a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61b4a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="61b4a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61b4a-107">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="61b4a-107">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="61b4a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="61b4a-108">Members</span></span>
|<span data-ttu-id="61b4a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="61b4a-109">Member</span></span>|<span data-ttu-id="61b4a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="61b4a-110">Value</span></span>|<span data-ttu-id="61b4a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="61b4a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61b4a-112">resourceScope</span><span class="sxs-lookup"><span data-stu-id="61b4a-112">resourceScope</span></span>|<span data-ttu-id="61b4a-113">,0</span><span class="sxs-lookup"><span data-stu-id="61b4a-113">0</span></span>|<span data-ttu-id="61b4a-114">Permite atribuições para o ResourceScopes especificado.</span><span class="sxs-lookup"><span data-stu-id="61b4a-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="61b4a-115">objectdevices</span><span class="sxs-lookup"><span data-stu-id="61b4a-115">allDevices</span></span>|<span data-ttu-id="61b4a-116">1 </span><span class="sxs-lookup"><span data-stu-id="61b4a-116">1</span></span>|<span data-ttu-id="61b4a-117">Permitir atribuições de todos os dispositivos do Intune.</span><span class="sxs-lookup"><span data-stu-id="61b4a-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="61b4a-118">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="61b4a-118">allLicensedUsers</span></span>|<span data-ttu-id="61b4a-119">2 </span><span class="sxs-lookup"><span data-stu-id="61b4a-119">2</span></span>|<span data-ttu-id="61b4a-120">Permitir atribuições a todos os usuários licenciados do Intune.</span><span class="sxs-lookup"><span data-stu-id="61b4a-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="61b4a-121">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="61b4a-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="61b4a-122">3 </span><span class="sxs-lookup"><span data-stu-id="61b4a-122">3</span></span>|<span data-ttu-id="61b4a-123">Permitir atribuições de todos os dispositivos do Intune e usuários licenciados.</span><span class="sxs-lookup"><span data-stu-id="61b4a-123">Allow assignments to all Intune devices and licensed users.</span></span>|



