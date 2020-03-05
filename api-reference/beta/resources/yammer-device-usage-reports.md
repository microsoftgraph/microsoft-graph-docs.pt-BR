---
title: Relatórios de uso de dispositivos do Yammer
description: Os relatórios de uso do dispositivo para o Yammer fornecem informações sobre quais dispositivos seus usuários utilizam para se envolver no Yammer. Você pode exibir o número de usuários por tipo de dispositivo em um período de tempo selecionado e exibir detalhes por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 02d5f3bcb71b343b0406536d77d80d477cc71223
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519047"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="0fcdd-104">Relatórios de uso de dispositivos do Yammer</span><span class="sxs-lookup"><span data-stu-id="0fcdd-104">Yammer device usage reports</span></span>

<span data-ttu-id="0fcdd-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0fcdd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fcdd-106">Os relatórios de uso do dispositivo para o Yammer fornecem informações sobre quais dispositivos seus usuários utilizam para se envolver no Yammer.</span><span class="sxs-lookup"><span data-stu-id="0fcdd-106">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="0fcdd-107">Você pode exibir o número de usuários por tipo de dispositivo em um período de tempo selecionado e exibir detalhes por usuário.</span><span class="sxs-lookup"><span data-stu-id="0fcdd-107">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="0fcdd-108">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="0fcdd-108">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="0fcdd-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="0fcdd-109">Reports</span></span>

| <span data-ttu-id="0fcdd-110">Função</span><span class="sxs-lookup"><span data-stu-id="0fcdd-110">Function</span></span>                                 | <span data-ttu-id="0fcdd-111">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="0fcdd-111">CSV return type</span></span> | <span data-ttu-id="0fcdd-112">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="0fcdd-112">JSON return type</span></span>                         | <span data-ttu-id="0fcdd-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fcdd-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="0fcdd-114">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="0fcdd-114">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="0fcdd-115">Stream</span><span class="sxs-lookup"><span data-stu-id="0fcdd-115">Stream</span></span>          | [<span data-ttu-id="0fcdd-116">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="0fcdd-116">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="0fcdd-117">Obtenha dados sobre o uso do dispositivo Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="0fcdd-117">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="0fcdd-118">Obter contagens de usuários de distribuição</span><span class="sxs-lookup"><span data-stu-id="0fcdd-118">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="0fcdd-119">Fluxo</span><span class="sxs-lookup"><span data-stu-id="0fcdd-119">Stream</span></span>          | [<span data-ttu-id="0fcdd-120">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="0fcdd-120">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="0fcdd-121">Obtenha o número de usuários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0fcdd-121">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="0fcdd-122">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="0fcdd-122">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="0fcdd-123">Fluxo</span><span class="sxs-lookup"><span data-stu-id="0fcdd-123">Stream</span></span>          | [<span data-ttu-id="0fcdd-124">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="0fcdd-124">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="0fcdd-125">Obtenha o número de usuários diários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0fcdd-125">Get the number of daily users by device type.</span></span> |
