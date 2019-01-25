---
title: Relatórios de uso de dispositivos do Yammer
description: Os relatórios de uso de dispositivos paro Yammer fornecem informações sobre quais dispositivos seus usuários utilizam para conectar no Yammer. Você pode exibir o número de usuários por tipo de dispositivo em um período de tempo selecionado e visualizar dados por usuário.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: f5b24d6d235a8719f5f4b7df0389b5e5971dd8cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521863"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="d0045-104">Relatórios de uso de dispositivos do Yammer</span><span class="sxs-lookup"><span data-stu-id="d0045-104">Yammer device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0045-105">Os relatórios de uso de dispositivos paro Yammer fornecem informações sobre quais dispositivos seus usuários utilizam para conectar no Yammer.</span><span class="sxs-lookup"><span data-stu-id="d0045-105">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="d0045-106">Você pode exibir o número de usuários por tipo de dispositivo em um período de tempo selecionado e visualizar dados por usuário.</span><span class="sxs-lookup"><span data-stu-id="d0045-106">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="d0045-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="d0045-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="d0045-108">Relatórios</span><span class="sxs-lookup"><span data-stu-id="d0045-108">Reports</span></span>

| <span data-ttu-id="d0045-109">Função</span><span class="sxs-lookup"><span data-stu-id="d0045-109">Function</span></span>                                 | <span data-ttu-id="d0045-110">Tipo de retorno de CSV</span><span class="sxs-lookup"><span data-stu-id="d0045-110">CSV return type</span></span> | <span data-ttu-id="d0045-111">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="d0045-111">JSON return type</span></span>                         | <span data-ttu-id="d0045-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0045-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="d0045-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="d0045-113">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="d0045-114">Stream</span><span class="sxs-lookup"><span data-stu-id="d0045-114">Stream</span></span>          | [<span data-ttu-id="d0045-115">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="d0045-115">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="d0045-116">Obtenha dados sobre o uso do dispositivo Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="d0045-116">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="d0045-117">Obter contagens de usuários de distribuição</span><span class="sxs-lookup"><span data-stu-id="d0045-117">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="d0045-118">Fluxo</span><span class="sxs-lookup"><span data-stu-id="d0045-118">Stream</span></span>          | [<span data-ttu-id="d0045-119">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="d0045-119">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="d0045-120">Obtenha o número de usuários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0045-120">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="d0045-121">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="d0045-121">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="d0045-122">Stream</span><span class="sxs-lookup"><span data-stu-id="d0045-122">Stream</span></span>          | [<span data-ttu-id="d0045-123">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="d0045-123">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="d0045-124">Obtenha o número de usuários diários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0045-124">Get the number of daily users by device type.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
