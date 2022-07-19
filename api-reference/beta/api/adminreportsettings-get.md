---
title: Obter adminReportSettings
description: Obtenha as configurações no nível do locatário para relatórios do Microsoft 365.
ms.localizationpriority: medium
author: qiwhuang
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: b9edf2396cd3409e794386f08eb4a124ce65d892
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856495"
---
# <a name="get-adminreportsettings"></a>Obter adminReportSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha as configurações no nível do locatário para relatórios do Microsoft 365.

> **Nota:** Para obter detalhes sobre diferentes exibições e nomes de relatório, consulte [Relatórios do Microsoft 365 no centro de administração – Microsoft 365 Apps uso](/microsoft-365/admin/activity-reports/microsoft365-apps-usage).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)           |
|:---------------------------------------|:------------------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | ReportSettings.Read.All, ReportSettings.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                                        |
| Aplicativo                            | ReportSettings.Read.All, ReportSettings.ReadWrite.All |

> **Nota:** Para permissões delegadas para permitir que os aplicativos obtenham configurações de relatório em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada apropriada do Azure Active Directory. Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /admin/reportSettings
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um [objeto adminReportSettings](../resources/adminreportsettings.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "get_adminreportsettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/reportSettings
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.adminReportSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.adminReportSettings",
    "displayConcealedNames": true
  }
}
```
