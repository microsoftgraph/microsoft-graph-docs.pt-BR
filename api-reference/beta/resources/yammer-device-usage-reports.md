---
title: Relatórios de uso de dispositivos do Yammer
description: Os relatórios de uso do dispositivo para o Yammer fornecem informações sobre quais dispositivos seus usuários utilizam para se envolver no Yammer. Você pode exibir o número de usuários por tipo de dispositivo em um período de tempo selecionado e exibir detalhes por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 2c253d58d3f8b0bdd07d902bbcbe77af6a1666e9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342768"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="f6686-104">Relatórios de uso de dispositivos do Yammer</span><span class="sxs-lookup"><span data-stu-id="f6686-104">Yammer device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6686-105">Os relatórios de uso do dispositivo para o Yammer fornecem informações sobre quais dispositivos seus usuários utilizam para se envolver no Yammer.</span><span class="sxs-lookup"><span data-stu-id="f6686-105">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="f6686-106">Você pode exibir o número de usuários por tipo de dispositivo em um período de tempo selecionado e exibir detalhes por usuário.</span><span class="sxs-lookup"><span data-stu-id="f6686-106">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="f6686-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="f6686-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="f6686-108">Relatórios</span><span class="sxs-lookup"><span data-stu-id="f6686-108">Reports</span></span>

| <span data-ttu-id="f6686-109">Função</span><span class="sxs-lookup"><span data-stu-id="f6686-109">Function</span></span>                                 | <span data-ttu-id="f6686-110">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="f6686-110">CSV return type</span></span> | <span data-ttu-id="f6686-111">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="f6686-111">JSON return type</span></span>                         | <span data-ttu-id="f6686-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6686-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="f6686-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="f6686-113">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="f6686-114">Fluxo</span><span class="sxs-lookup"><span data-stu-id="f6686-114">Stream</span></span>          | [<span data-ttu-id="f6686-115">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="f6686-115">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="f6686-116">Obtenha dados sobre o uso do dispositivo Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="f6686-116">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="f6686-117">Obter contagens de usuários de distribuição</span><span class="sxs-lookup"><span data-stu-id="f6686-117">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="f6686-118">Fluxo</span><span class="sxs-lookup"><span data-stu-id="f6686-118">Stream</span></span>          | [<span data-ttu-id="f6686-119">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="f6686-119">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="f6686-120">Obtenha o número de usuários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f6686-120">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="f6686-121">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="f6686-121">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="f6686-122">Fluxo</span><span class="sxs-lookup"><span data-stu-id="f6686-122">Stream</span></span>          | [<span data-ttu-id="f6686-123">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="f6686-123">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="f6686-124">Obtenha o número de usuários diários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f6686-124">Get the number of daily users by device type.</span></span> |
