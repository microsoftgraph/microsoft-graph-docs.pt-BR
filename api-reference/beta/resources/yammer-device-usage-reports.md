---
title: Relatórios de uso de dispositivos do Yammer
description: Os relatórios de uso do dispositivo para o Yammer fornecem informações sobre quais dispositivos seus usuários utilizam para se envolver no Yammer. Você pode exibir o número de usuários por tipo de dispositivo em um período de tempo selecionado e exibir detalhes por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 57dcba3a91b15b4980d9e76b7aad6251008f5966
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555288"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="84d8f-104">Relatórios de uso de dispositivos do Yammer</span><span class="sxs-lookup"><span data-stu-id="84d8f-104">Yammer device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84d8f-105">Os relatórios de uso do dispositivo para o Yammer fornecem informações sobre quais dispositivos seus usuários utilizam para se envolver no Yammer.</span><span class="sxs-lookup"><span data-stu-id="84d8f-105">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="84d8f-106">Você pode exibir o número de usuários por tipo de dispositivo em um período de tempo selecionado e exibir detalhes por usuário.</span><span class="sxs-lookup"><span data-stu-id="84d8f-106">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="84d8f-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="84d8f-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="84d8f-108">Relatórios</span><span class="sxs-lookup"><span data-stu-id="84d8f-108">Reports</span></span>

| <span data-ttu-id="84d8f-109">Função</span><span class="sxs-lookup"><span data-stu-id="84d8f-109">Function</span></span>                                 | <span data-ttu-id="84d8f-110">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="84d8f-110">CSV return type</span></span> | <span data-ttu-id="84d8f-111">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="84d8f-111">JSON return type</span></span>                         | <span data-ttu-id="84d8f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="84d8f-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="84d8f-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="84d8f-113">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="84d8f-114">Fluxo</span><span class="sxs-lookup"><span data-stu-id="84d8f-114">Stream</span></span>          | [<span data-ttu-id="84d8f-115">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="84d8f-115">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="84d8f-116">Obtenha dados sobre o uso do dispositivo Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="84d8f-116">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="84d8f-117">Obter contagens de usuários de distribuição</span><span class="sxs-lookup"><span data-stu-id="84d8f-117">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="84d8f-118">Fluxo</span><span class="sxs-lookup"><span data-stu-id="84d8f-118">Stream</span></span>          | [<span data-ttu-id="84d8f-119">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="84d8f-119">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="84d8f-120">Obtenha o número de usuários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84d8f-120">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="84d8f-121">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="84d8f-121">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="84d8f-122">Fluxo</span><span class="sxs-lookup"><span data-stu-id="84d8f-122">Stream</span></span>          | [<span data-ttu-id="84d8f-123">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="84d8f-123">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="84d8f-124">Obtenha o número de usuários diários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84d8f-124">Get the number of daily users by device type.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
