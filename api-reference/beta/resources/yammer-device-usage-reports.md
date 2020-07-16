---
title: Relatórios de uso de dispositivos do Yammer
description: Os relatórios de uso do dispositivo para o Yammer fornecem informações sobre quais dispositivos seus usuários utilizam para se envolver no Yammer. Você pode exibir o número de usuários por tipo de dispositivo em um período de tempo selecionado e exibir detalhes por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 126ac55083fa730103c5584c5848490bf3cb267e
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897152"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="5d571-104">Relatórios de uso de dispositivos do Yammer</span><span class="sxs-lookup"><span data-stu-id="5d571-104">Yammer device usage reports</span></span>

<span data-ttu-id="5d571-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d571-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d571-106">Os relatórios de uso do dispositivo para o Yammer fornecem informações sobre quais dispositivos seus usuários utilizam para se envolver no Yammer.</span><span class="sxs-lookup"><span data-stu-id="5d571-106">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="5d571-107">Você pode exibir o número de usuários por tipo de dispositivo em um período de tempo selecionado e exibir detalhes por usuário.</span><span class="sxs-lookup"><span data-stu-id="5d571-107">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="5d571-108">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="5d571-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="5d571-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="5d571-109">Reports</span></span>

| <span data-ttu-id="5d571-110">Função</span><span class="sxs-lookup"><span data-stu-id="5d571-110">Function</span></span>                                 | <span data-ttu-id="5d571-111">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="5d571-111">CSV return type</span></span> | <span data-ttu-id="5d571-112">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="5d571-112">JSON return type</span></span>                         | <span data-ttu-id="5d571-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d571-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="5d571-114">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="5d571-114">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="5d571-115">Stream</span><span class="sxs-lookup"><span data-stu-id="5d571-115">Stream</span></span>          | [<span data-ttu-id="5d571-116">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="5d571-116">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="5d571-117">Obtenha dados sobre o uso do dispositivo Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="5d571-117">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="5d571-118">Obter contagens de usuários de distribuição</span><span class="sxs-lookup"><span data-stu-id="5d571-118">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="5d571-119">Fluxo</span><span class="sxs-lookup"><span data-stu-id="5d571-119">Stream</span></span>          | [<span data-ttu-id="5d571-120">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="5d571-120">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="5d571-121">Obtenha o número de usuários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5d571-121">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="5d571-122">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="5d571-122">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="5d571-123">Fluxo</span><span class="sxs-lookup"><span data-stu-id="5d571-123">Stream</span></span>          | [<span data-ttu-id="5d571-124">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="5d571-124">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="5d571-125">Obtenha o número de usuários diários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5d571-125">Get the number of daily users by device type.</span></span> |
