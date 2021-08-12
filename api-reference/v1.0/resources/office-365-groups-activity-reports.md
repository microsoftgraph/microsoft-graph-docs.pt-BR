---
title: Microsoft 365 de atividades de grupos
description: Você pode usar os relatórios de atividades grupos para obter informações sobre a atividade de Microsoft 365 grupos em sua organização e ver quantos grupos de Microsoft 365 estão sendo criados e usados.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 814b66d419fea4d06cbf16158298fac81c644ba794f3c0f85a8c32e2996d776f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54174917"
---
# <a name="microsoft-365-groups-activity-reports"></a>Microsoft 365 de atividades de grupos

Namespace: microsoft.graph

Você pode usar os relatórios de atividades grupos para obter informações sobre a atividade de Microsoft 365 grupos em sua organização e ver quantos grupos de Microsoft 365 estão sendo criados e usados.

> **Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - Microsoft 365 grupos](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno | Descrição                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [Obter dados de grupo](../api/reportroot-getoffice365groupsactivitydetail.md) | Fluxo          | Obter detalhes sobre Microsoft 365 grupos por grupo. |
| [Obter contagens de atividades](../api/reportroot-getoffice365groupsactivitycounts.md) | Fluxo          | Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo. |
| [Obter contagens de grupo](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Fluxo          | Obtenha o número total diário de grupos e quantos deles estavam ativos com base em conversas de email, postagens do Yammer e atividades de arquivo do SharePoint. |
| [Obter armazenamento](../api/reportroot-getoffice365groupsactivitystorage.md) | Fluxo          | Obtenha o armazenamento total usado em todas as caixas de correio de grupo e sites de grupo. |
| [Obter contagens de arquivo](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Fluxo          | Obter o número total de arquivos e quantos deles estavam ativos em todos os sites de grupo associados a um Microsoft 365 grupo. |

