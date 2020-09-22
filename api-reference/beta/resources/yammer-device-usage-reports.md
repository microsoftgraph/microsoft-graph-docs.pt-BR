---
title: Relatórios de uso de dispositivos do Yammer
description: Os relatórios de uso do dispositivo para o Yammer fornecem informações sobre quais dispositivos seus usuários utilizam para se envolver no Yammer. Você pode exibir o número de usuários por tipo de dispositivo em um período de tempo selecionado e exibir detalhes por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: c23e67c22189ff08468b44b1993034616dd74e27
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070412"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="47aca-104">Relatórios de uso de dispositivos do Yammer</span><span class="sxs-lookup"><span data-stu-id="47aca-104">Yammer device usage reports</span></span>

<span data-ttu-id="47aca-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47aca-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47aca-106">Os relatórios de uso do dispositivo para o Yammer fornecem informações sobre quais dispositivos seus usuários utilizam para se envolver no Yammer.</span><span class="sxs-lookup"><span data-stu-id="47aca-106">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="47aca-107">Você pode exibir o número de usuários por tipo de dispositivo em um período de tempo selecionado e exibir detalhes por usuário.</span><span class="sxs-lookup"><span data-stu-id="47aca-107">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="47aca-108">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="47aca-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="47aca-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="47aca-109">Reports</span></span>

| <span data-ttu-id="47aca-110">Função</span><span class="sxs-lookup"><span data-stu-id="47aca-110">Function</span></span>                                 | <span data-ttu-id="47aca-111">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="47aca-111">CSV return type</span></span> | <span data-ttu-id="47aca-112">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="47aca-112">JSON return type</span></span>                         | <span data-ttu-id="47aca-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="47aca-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="47aca-114">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="47aca-114">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="47aca-115">Fluxo</span><span class="sxs-lookup"><span data-stu-id="47aca-115">Stream</span></span>          | [<span data-ttu-id="47aca-116">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="47aca-116">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="47aca-117">Obtenha dados sobre o uso do dispositivo Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="47aca-117">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="47aca-118">Obter contagens de usuários de distribuição</span><span class="sxs-lookup"><span data-stu-id="47aca-118">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="47aca-119">Fluxo</span><span class="sxs-lookup"><span data-stu-id="47aca-119">Stream</span></span>          | [<span data-ttu-id="47aca-120">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="47aca-120">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="47aca-121">Obtenha o número de usuários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47aca-121">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="47aca-122">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="47aca-122">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="47aca-123">Fluxo</span><span class="sxs-lookup"><span data-stu-id="47aca-123">Stream</span></span>          | [<span data-ttu-id="47aca-124">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="47aca-124">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="47aca-125">Obtenha o número de usuários diários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47aca-125">Get the number of daily users by device type.</span></span> |


