---
title: Criar uma configuração de diretório
description: Use essa API para criar uma nova definição, com base em modelos de disponíveis no directorySettingTemplates. Essas configurações podem ser no nível do locatário ou em um nível de objeto (atualmente somente para grupos). A solicitação de criação deve fornecer settingValues para todas as configurações definidas no modelo. Para configurações específicas de grupo, somente a configuração que controlam se os membros de um grupo podem convidar usuários convidados pode ser definido. Depois que a capacidade de adicionar usuários convidados a um grupo estiver disponível, isso orientará esse comportamento.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6754e8e4210da0161a6f0cd790dc355e4788e121
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921763"
---
# <a name="create-a-directory-setting"></a>Criar uma configuração de diretório

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Use essa API para criar uma nova definição, com base em modelos de disponíveis no directorySettingTemplates. Essas configurações podem ser no nível do locatário ou em um nível de objeto (atualmente somente para grupos). A solicitação de criação deve fornecer settingValues para todas as configurações definidas no modelo. Para configurações específicas de grupo, somente a configuração que controlam se os membros de um grupo podem convidar usuários convidados pode ser definido. Depois que a capacidade de adicionar usuários convidados a um grupo estiver disponível, isso orientará esse comportamento.

> **Observação**: A versão de /beta desse API é só se aplica aos grupos. A versão de /v1.0 desse API foi renomeada para *criar groupSettings*.

Para obter uma lista de modelos e as propriedades que eles oferecem suporte na versão beta, use uma [consulta directorySettingTemplate](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta). (Para os pontos de extremidade v 1.0, chamada [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | {token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do objeto [directorySetting](../resources/directorysetting.md) .  No entanto, o nome de exibição para a configuração será definido com base no nome do modelo de configurações referenciado.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `201 Created` objeto response de código e [directorySetting](../resources/directorysetting.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_settings"
}-->
```http
POST https://graph.microsoft.com/beta/settings
Content-type: application/json
Content-length: 222

{
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
No corpo da solicitação, fornece uma representação JSON do objeto [directorySetting](../resources/directorysetting.md) .
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
    "@odata.context": "https://graph.microsoft.com/stagingbeta/$metadata#settings/$entity",
    "id": "id-value",
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
