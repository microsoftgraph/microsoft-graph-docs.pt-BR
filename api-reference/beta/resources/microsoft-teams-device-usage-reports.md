---
title: Relatórios de uso de dispositivos do Microsoft Teams
description: 'Use os relatórios de uso de dispositivos do Microsoft Teams para obter informações sobre o uso de dispositivos do Microsoft Teams em sua organização. '
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d19df5132a67ac5862535a329eadbdff7044798c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457106"
---
# <a name="microsoft-teams-device-usage-reports"></a><span data-ttu-id="870ff-103">Relatórios de uso de dispositivos do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="870ff-103">Microsoft Teams device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="870ff-104">Use os relatórios de uso de dispositivos do Microsoft Teams para obter informações sobre o uso de dispositivos do Microsoft Teams em sua organização.</span><span class="sxs-lookup"><span data-stu-id="870ff-104">Use the Microsoft Teams device usage reports to get insights into the Microsoft Teams device usage in your organization.</span></span> 

## <a name="methods"></a><span data-ttu-id="870ff-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="870ff-105">Methods</span></span>

| <span data-ttu-id="870ff-106">Método</span><span class="sxs-lookup"><span data-stu-id="870ff-106">Method</span></span>                                   | <span data-ttu-id="870ff-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="870ff-107">Return Type</span></span>                              | <span data-ttu-id="870ff-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="870ff-108">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="870ff-109">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="870ff-109">Get user detail</span></span>](../api/reportroot-getteamsdeviceusageuserdetail.md) | [<span data-ttu-id="870ff-110">teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="870ff-110">teamsDeviceUsageUserDetail</span></span>](../resources/teamsdeviceusageuserdetail.md) | <span data-ttu-id="870ff-111">Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário.</span><span class="sxs-lookup"><span data-stu-id="870ff-111">Get details about Microsoft Teams device usage by user.</span></span> |
| [<span data-ttu-id="870ff-112">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="870ff-112">Get user counts</span></span>](../api/reportroot-getteamsdeviceusageusercounts.md) | [<span data-ttu-id="870ff-113">teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="870ff-113">teamsDeviceUsageUserCounts</span></span>](../resources/teamsdeviceusageusercounts.md) | <span data-ttu-id="870ff-114">Obtém o número de usuários exclusivos diários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="870ff-114">Get the number of daily unique users by device type.</span></span> |
| [<span data-ttu-id="870ff-115">Obter contagens de usuários de distribuição</span><span class="sxs-lookup"><span data-stu-id="870ff-115">Get distribution user counts</span></span>](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [<span data-ttu-id="870ff-116">teamsDeviceUsagedistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="870ff-116">teamsDeviceUsagedistributionUserCounts</span></span>](../resources/teamsdeviceusagedistributionusercounts.md) | <span data-ttu-id="870ff-117">Obtém o número de usuários exclusivos por tipo de dispositivo no período de tempo selecionado.</span><span class="sxs-lookup"><span data-stu-id="870ff-117">Get the number of unique users by device type over the selected time period.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
