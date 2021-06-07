---
title: Tipo de número sharedPCAccountDeletionPolicyType
description: Valores possíveis para quando contas são excluídas em um computador compartilhado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a3b4245ccf1a5a03d8b2142b65bfed69685de254
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751717"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="10257-103">Tipo de número sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="10257-103">sharedPCAccountDeletionPolicyType enum type</span></span>

<span data-ttu-id="10257-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10257-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10257-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="10257-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10257-106">Valores possíveis para quando contas são excluídas em um computador compartilhado.</span><span class="sxs-lookup"><span data-stu-id="10257-106">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="10257-107">Membros</span><span class="sxs-lookup"><span data-stu-id="10257-107">Members</span></span>
|<span data-ttu-id="10257-108">Membro</span><span class="sxs-lookup"><span data-stu-id="10257-108">Member</span></span>|<span data-ttu-id="10257-109">Valor</span><span class="sxs-lookup"><span data-stu-id="10257-109">Value</span></span>|<span data-ttu-id="10257-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="10257-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10257-111">immediate</span><span class="sxs-lookup"><span data-stu-id="10257-111">immediate</span></span>|<span data-ttu-id="10257-112">0</span><span class="sxs-lookup"><span data-stu-id="10257-112">0</span></span>|<span data-ttu-id="10257-113">Exclua imediatamente.</span><span class="sxs-lookup"><span data-stu-id="10257-113">Delete immediately.</span></span>|
|<span data-ttu-id="10257-114">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="10257-114">diskSpaceThreshold</span></span>|<span data-ttu-id="10257-115">1</span><span class="sxs-lookup"><span data-stu-id="10257-115">1</span></span>|<span data-ttu-id="10257-116">Excluir no limite de espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="10257-116">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="10257-117">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="10257-117">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="10257-118">2</span><span class="sxs-lookup"><span data-stu-id="10257-118">2</span></span>|<span data-ttu-id="10257-119">Excluir no limite de espaço em disco ou no limite inativo.</span><span class="sxs-lookup"><span data-stu-id="10257-119">Delete at disk space threshold or inactive threshold.</span></span>|




