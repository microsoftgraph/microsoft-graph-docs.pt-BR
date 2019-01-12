---
title: tipo de enum deviceManagementExchangeAccessState
description: Estado de acesso do Exchange de dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dbfa7b9396a1100f2e3c7e4e78cf697233d840cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947012"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="a5123-103">tipo de enum deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="a5123-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="a5123-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a5123-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5123-105">Estado de acesso do Exchange de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a5123-105">Device Exchange Access State.</span></span>
## <a name="members"></a><span data-ttu-id="a5123-106">Membros</span><span class="sxs-lookup"><span data-stu-id="a5123-106">Members</span></span>
|<span data-ttu-id="a5123-107">Membro</span><span class="sxs-lookup"><span data-stu-id="a5123-107">Member</span></span>|<span data-ttu-id="a5123-108">Valor</span><span class="sxs-lookup"><span data-stu-id="a5123-108">Value</span></span>|<span data-ttu-id="a5123-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5123-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5123-110">nenhum</span><span class="sxs-lookup"><span data-stu-id="a5123-110">none</span></span>|<span data-ttu-id="a5123-111">0</span><span class="sxs-lookup"><span data-stu-id="a5123-111">0</span></span>|<span data-ttu-id="a5123-112">Nenhum estado de acesso descoberto do Exchange</span><span class="sxs-lookup"><span data-stu-id="a5123-112">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="a5123-113">unknown</span><span class="sxs-lookup"><span data-stu-id="a5123-113">unknown</span></span>|<span data-ttu-id="a5123-114">1</span><span class="sxs-lookup"><span data-stu-id="a5123-114">1</span></span>|<span data-ttu-id="a5123-115">O estado de acesso de dispositivo para o Exchange é desconhecido</span><span class="sxs-lookup"><span data-stu-id="a5123-115">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="a5123-116">permitido</span><span class="sxs-lookup"><span data-stu-id="a5123-116">allowed</span></span>|<span data-ttu-id="a5123-117">2</span><span class="sxs-lookup"><span data-stu-id="a5123-117">2</span></span>|<span data-ttu-id="a5123-118">Dispositivo tem acesso ao Exchange</span><span class="sxs-lookup"><span data-stu-id="a5123-118">Device has access to Exchange</span></span>|
|<span data-ttu-id="a5123-119">bloqueado</span><span class="sxs-lookup"><span data-stu-id="a5123-119">blocked</span></span>|<span data-ttu-id="a5123-120">3</span><span class="sxs-lookup"><span data-stu-id="a5123-120">3</span></span>|<span data-ttu-id="a5123-121">Dispositivo está bloqueado no Exchange</span><span class="sxs-lookup"><span data-stu-id="a5123-121">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="a5123-122">em quarentena</span><span class="sxs-lookup"><span data-stu-id="a5123-122">quarantined</span></span>|<span data-ttu-id="a5123-123">4</span><span class="sxs-lookup"><span data-stu-id="a5123-123">4</span></span>|<span data-ttu-id="a5123-124">Dispositivo será colocada em quarentena no Exchange</span><span class="sxs-lookup"><span data-stu-id="a5123-124">Device is Quarantined in Exchange</span></span>|



