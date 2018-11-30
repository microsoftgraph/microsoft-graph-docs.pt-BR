---
title: tipo de enum sharedPCAccountDeletionPolicyType
description: Valores possíveis para quando as contas são excluídas em um PC compartilhado.
ms.openlocfilehash: bf58a865dcb970760c4cf5284533cd833fcf9304
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037044"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="cb3e3-103">tipo de enum sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="cb3e3-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="cb3e3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cb3e3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb3e3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cb3e3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb3e3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cb3e3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb3e3-107">Valores possíveis para quando as contas são excluídas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="cb3e3-107">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="cb3e3-108">Membros</span><span class="sxs-lookup"><span data-stu-id="cb3e3-108">Members</span></span>
|<span data-ttu-id="cb3e3-109">Membro</span><span class="sxs-lookup"><span data-stu-id="cb3e3-109">Member</span></span>|<span data-ttu-id="cb3e3-110">Valor</span><span class="sxs-lookup"><span data-stu-id="cb3e3-110">Value</span></span>|<span data-ttu-id="cb3e3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb3e3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb3e3-112">imediata</span><span class="sxs-lookup"><span data-stu-id="cb3e3-112">immediate</span></span>|<span data-ttu-id="cb3e3-113">0</span><span class="sxs-lookup"><span data-stu-id="cb3e3-113">0</span></span>|<span data-ttu-id="cb3e3-114">Exclua imediatamente.</span><span class="sxs-lookup"><span data-stu-id="cb3e3-114">Delete immediately.</span></span>|
|<span data-ttu-id="cb3e3-115">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="cb3e3-115">diskSpaceThreshold</span></span>|<span data-ttu-id="cb3e3-116">1</span><span class="sxs-lookup"><span data-stu-id="cb3e3-116">1</span></span>|<span data-ttu-id="cb3e3-117">Exclua cada limite de espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="cb3e3-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="cb3e3-118">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="cb3e3-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="cb3e3-119">2</span><span class="sxs-lookup"><span data-stu-id="cb3e3-119">2</span></span>|<span data-ttu-id="cb3e3-120">Exclua cada limite de espaço em disco ou o limite inativa.</span><span class="sxs-lookup"><span data-stu-id="cb3e3-120">Delete at disk space threshold or inactive threshold.</span></span>|





