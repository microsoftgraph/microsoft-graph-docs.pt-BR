---
title: tipo de enum sharedPCAccountDeletionPolicyType
description: Valores possíveis para quando as contas são excluídas em um PC compartilhado.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 645cd3dfd4121c6c9bdd9d57a0dc3b63723cc461
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415163"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="3f477-103">tipo de enum sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="3f477-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="3f477-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="3f477-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3f477-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3f477-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3f477-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="3f477-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f477-107">Valores possíveis para quando as contas são excluídas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="3f477-107">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="3f477-108">Membros</span><span class="sxs-lookup"><span data-stu-id="3f477-108">Members</span></span>
|<span data-ttu-id="3f477-109">Membro</span><span class="sxs-lookup"><span data-stu-id="3f477-109">Member</span></span>|<span data-ttu-id="3f477-110">Valor</span><span class="sxs-lookup"><span data-stu-id="3f477-110">Value</span></span>|<span data-ttu-id="3f477-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f477-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f477-112">imediata</span><span class="sxs-lookup"><span data-stu-id="3f477-112">immediate</span></span>|<span data-ttu-id="3f477-113">0</span><span class="sxs-lookup"><span data-stu-id="3f477-113">0</span></span>|<span data-ttu-id="3f477-114">Exclua imediatamente.</span><span class="sxs-lookup"><span data-stu-id="3f477-114">Delete immediately.</span></span>|
|<span data-ttu-id="3f477-115">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="3f477-115">diskSpaceThreshold</span></span>|<span data-ttu-id="3f477-116">1</span><span class="sxs-lookup"><span data-stu-id="3f477-116">1</span></span>|<span data-ttu-id="3f477-117">Exclua cada limite de espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="3f477-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="3f477-118">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="3f477-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="3f477-119">2</span><span class="sxs-lookup"><span data-stu-id="3f477-119">2</span></span>|<span data-ttu-id="3f477-120">Exclua cada limite de espaço em disco ou o limite inativa.</span><span class="sxs-lookup"><span data-stu-id="3f477-120">Delete at disk space threshold or inactive threshold.</span></span>|




