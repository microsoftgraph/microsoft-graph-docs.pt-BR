---
title: Atualizar adminReportSettings
description: Atualize as configurações no nível do locatário para relatórios do Microsoft 365.
ms.localizationpriority: medium
author: qiwhuang
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 0fb9ed8d8e80bf195e3d63f5139ca6498246fc48
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856494"
---
# <a name="update-adminreportsettings"></a>Atualizar adminReportSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as configurações no nível do locatário para relatórios do Microsoft 365.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|----------------------------------------|---------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | ReportSettings.ReadWrite.All                |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | ReportSettings.ReadWrite.All                |

> **Nota:** Para permissões delegadas para permitir que os aplicativos atualizem as configurações de relatório em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada apropriada do Azure Active Directory. Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } --> 
```http
PATCH /admin/reportSettings
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                |
| :------------ | :--------------------------|
| Autorização | {token} de portador. Obrigatório.  |
| Content-Type  | application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| Propriedade       | Tipo           | Descrição                                 |
| -------------- | -------------- | ------------------------------------------- |
| displayConcealedNames | Booliano | Se definido como `true`, todos os relatórios ocultarão informações do usuário, como nomes de usuário, grupos e sites. Se `false`, todos os relatórios mostrarão informações identificáveis. Essa propriedade representa uma configuração no Centro de administração do Microsoft 365. Obrigatório. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

A seguir está um exemplo de uma solicitação que atualiza uma configuração no nível do locatário para relatórios do Microsoft 365.

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "update_adminreportsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/admin/reportSettings
Content-Type: application/json
Content-length: 37

{
  "displayConcealedNames": true
}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
