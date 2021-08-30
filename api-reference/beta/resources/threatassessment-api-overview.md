---
title: Usar a API de avaliação de ameaças do Microsoft Graph
description: O Microsoft Graph permite que seu aplicativo obtenha acesso autorizado aos dados de avaliação de ameaças da organização.
ms.localizationpriority: high
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 8a0704d4e601bfe7c8750c376fdbd4c20b9888f5
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695602"
---
# <a name="use-the-microsoft-graph-threat-assessment-api"></a>Usar a API de avaliação de ameaças do Microsoft Graph

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A API de avaliação de ameaças do Microsoft Graph ajuda as organizações a avaliar a ameaça recebida por qualquer usuário em um locatário. Isso permite que os clientes relatem emails de spam, URLs de phishing ou anexos de malware recebidos na Microsoft. Os resultados da verificação de política e os resultados ao verificar novamente, podem ajudar os administradores de locatários a entender o veredicto da verificação de ameaças e ajustar sua política organizacional.

## <a name="authorization"></a>Autorização

O Microsoft Graph controla o acesso a recursos por meio de permissões. Você deve especificar as permissões necessárias para acessar os recursos de avaliação de ameaças. Normalmente, você deve especificar as permissões no portal do Azure Active Directory (Azure AD). Para saber mais, confira [Referência de permissões do Microsoft Graph](/graph/permissions-reference) e [Permissões de avaliação de ameaças](/graph/permissions-reference#threat-assessment-permissions).

## <a name="common-use-cases"></a>Casos de uso comuns

A API de avaliação de ameaças do Microsoft Graph fornece métodos para listar, criar e obter solicitações de avaliação de ameaças e recuperar os resultados da avaliação.

| Casos de uso | Recursos REST | Confira também |
|:----------|:---------------|:---------|
| Listar, criar e obter solicitações de avaliação de ameaças | [threatAssessmentRequest](../resources/threatassessmentrequest.md)<br> [mailAssessmentRequest](../resources/mailAssessmentRequest.md)<br> [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md)<br> [fileAssessmentRequest](../resources/fileAssessmentRequest.md)<br> [urlAssessmentRequest](../resources/urlAssessmentRequest.md)<br> | [Create threatAssessmentRequest](../api/informationprotection-post-threatassessmentrequests.md)<br> [Get threatAssessmentRequest](../api/threatassessmentrequest-get.md)<br> [List threatAssessmentRequest](../api/informationprotection-list-threatassessmentrequests.md) |
| Obter os resultados da avaliação de ameaças | [threatAssessmentResult](../resources/threatassessmentresult.md) | [Get threatAssessmentResult](../api/threatassessmentrequest-get.md#example-5-expand-threat-assessment-results-for-a-request)|

## <a name="next-steps"></a>Próximas etapas

Os recursos de avaliação de ameaças e as APIs podem abrir novas maneiras de se envolver com os usuários e gerenciar suas experiências com o Microsoft Graph. Para saber mais:

- Faça um drill down em [métodos](../resources/threatassessmentrequest.md#methods), [propriedades](../resources/threatassessmentrequest.md#properties) e [relações](../resources/threatassessmentrequest.md#relationships) dos recursos de [solicitação de avaliação de ameaças](../resources/threatassessmentrequest.md) e de[resultado da avaliação de ameaças](../resources/threatAssessmentResult.md).
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).


