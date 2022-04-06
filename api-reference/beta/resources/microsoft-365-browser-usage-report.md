---
title: Microsoft 365 de uso do navegador
description: Use os Microsoft 365 de uso do navegador para obter informações sobre o uso de navegadores (Microsoft Edge, Versão Prévia do Microsoft Edge e Internet Explorer) em sua organização.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 8b0a0865ecd051d241f41844004ee247e0a57b17
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589647"
---
# <a name="microsoft-365-browser-usage-reports"></a>Microsoft 365 de uso do navegador

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use os Microsoft 365 de uso do navegador para obter informações sobre o uso de navegadores (Microsoft Edge, Versão Prévia do Microsoft Edge e Internet Explorer) em sua organização.

> **Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 Relatórios no centro de administração - uso do navegador da Microsoft](/microsoft-365/admin/activity-reports/browser-usage-report).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | --------------- | ---------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getbrowseruserdetail.md ) | Fluxo          | Stream | Obter o uso detalhado do navegador por usuário.  |
| [Obter contagens de usuários](../api/reportroot-getbrowserusercounts.md ) | Fluxo          | Stream |Obter a tendência no número de usuários ativos para cada navegador. |
| [Obter contagens de usuários de distribuição](../api/reportroot-getbrowserdistributionusercounts.md) | Fluxo          | Stream | Obter o número de usuários por navegador durante um período selecionado. |
