---
title: Relatórios de uso de dispositivos do Yammer
description: Os relatórios de uso de dispositivos do Yammer dão informações sobre quais dispositivos seus usuários utilizam para se envolver no Yammer. Você pode exibir o número de usuários por tipo de dispositivo durante um período de tempo selecionado e exibir detalhes por usuário.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 47dcdabb2230645ce2575fc573a99c37868c1919
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982429"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="7b1e3-104">Relatórios de uso de dispositivos do Yammer</span><span class="sxs-lookup"><span data-stu-id="7b1e3-104">Yammer device usage reports</span></span>

<span data-ttu-id="7b1e3-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b1e3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b1e3-106">Os relatórios de uso de dispositivos do Yammer dão informações sobre quais dispositivos seus usuários utilizam para se envolver no Yammer.</span><span class="sxs-lookup"><span data-stu-id="7b1e3-106">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="7b1e3-107">Você pode exibir o número de usuários por tipo de dispositivo durante um período de tempo selecionado e exibir detalhes por usuário.</span><span class="sxs-lookup"><span data-stu-id="7b1e3-107">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="7b1e3-108">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, confira [relatórios do Microsoft 365 - uso de dispositivos do Yammer.](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)</span><span class="sxs-lookup"><span data-stu-id="7b1e3-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="7b1e3-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="7b1e3-109">Reports</span></span>

| <span data-ttu-id="7b1e3-110">Função</span><span class="sxs-lookup"><span data-stu-id="7b1e3-110">Function</span></span>                                 | <span data-ttu-id="7b1e3-111">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="7b1e3-111">CSV return type</span></span> | <span data-ttu-id="7b1e3-112">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="7b1e3-112">JSON return type</span></span>                         | <span data-ttu-id="7b1e3-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b1e3-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="7b1e3-114">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="7b1e3-114">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="7b1e3-115">Fluxo</span><span class="sxs-lookup"><span data-stu-id="7b1e3-115">Stream</span></span>          | [<span data-ttu-id="7b1e3-116">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="7b1e3-116">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="7b1e3-117">Obtenha dados sobre o uso do dispositivo Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="7b1e3-117">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="7b1e3-118">Obter contagens de usuários de distribuição</span><span class="sxs-lookup"><span data-stu-id="7b1e3-118">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="7b1e3-119">Fluxo</span><span class="sxs-lookup"><span data-stu-id="7b1e3-119">Stream</span></span>          | [<span data-ttu-id="7b1e3-120">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="7b1e3-120">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="7b1e3-121">Obtenha o número de usuários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7b1e3-121">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="7b1e3-122">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="7b1e3-122">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="7b1e3-123">Fluxo</span><span class="sxs-lookup"><span data-stu-id="7b1e3-123">Stream</span></span>          | [<span data-ttu-id="7b1e3-124">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="7b1e3-124">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="7b1e3-125">Obtenha o número de usuários diários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7b1e3-125">Get the number of daily users by device type.</span></span> |


