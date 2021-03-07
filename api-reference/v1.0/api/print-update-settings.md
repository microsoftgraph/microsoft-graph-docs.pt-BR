---
title: Atualizar printSettings
description: Atualize as configurações de todo o locatário para o serviço de Impressão Universal.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: cc1af332871ef5d527bff235ef25906c4a739540
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516877"
---
# <a name="update-printsettings"></a>Atualizar printSettings
Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Atualize as configurações de todo o locatário para o serviço de Impressão Universal.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir. O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegado (conta corporativa ou de estudante)| PrintSettings.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/settings
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece os valores dos campos [printSettings relevantes](../resources/printsettings.md) que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|documentConversionEnabled|Booliano|Especifica se a conversão de documento está habilitada para o locatário. Se a conversão de documento estiver habilitada, o serviço de Impressão Universal converterá automaticamente documentos em um formato compatível com a impressora (por exemplo, XPS em PDF) quando necessário.|

## <a name="response"></a>Resposta

Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "update_printsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/settings
Content-type: application/json

{
  "documentConversionEnabled": true
}
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printSettings"
}
-->
``` http
HTTP/1.1 204 No Content
```

