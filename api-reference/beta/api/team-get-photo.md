---
title: Obter foto da equipe
description: Obter a foto (imagem) de uma equipe.
author: akjo
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8315dc28c4aa4c48efeb22b49409cdde1419fdbb
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695466"
---
# <a name="get-team-photo"></a>Obter foto da equipe

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha a foto (imagem) de uma equipe ou metadados da foto. Em geral, é uma prática recomendada primeiro tentar recuperar os metadados para o tamanho da foto que você deseja obter para garantir que o tamanho esteja disponível. Depois de recuperar os metadados, use o caminho `/$value` para obter os dados binários da foto.

Este método tenta primeiro recuperar a foto especificada do Microsoft 365. Se a foto não estiver disponível no Microsoft 365, ele tentará recuperar a foto do Azure Active Directory.

A seguir, são apresentados os tamanhos suportados de fotos em HD no Microsoft 365: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 e 648x648 pixels. As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.

Você pode obter os metadados da maior foto disponível ou, opcionalmente, especificar um tamanho para obter os metadados para esse tamanho de foto. Se o tamanho solicitado não estiver disponível, você poderá obter um tamanho menor. Por exemplo, se a maior foto carregada tiver 504x504 pixels, todos os tamanhos, exceto o de 648x648, estarão disponíveis para download. Se o tamanho especificado não estiver disponível no Microsoft 365 ou no Azure Active Directory, o tamanho 1x1 será retornado com o restante dos metadados.

> [!Note]
> Há um limite de 4 MB para o tamanho total da solicitação REST. Isso limita o tamanho da foto a menos de 4 MB.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | TeamSettings.Read.Group *, TeamSettings.ReadWrite.Group*, Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All  |

> **Observação**: Permissões marcadas com * usam [consentimento específico de recurso](https://aka.ms/teams-rsc).

> **Observação**: esta API dá suporte a permissões de administrador. Os administradores globais e os administradores de serviços do Microsoft Teams podem acessar equipes das quais não são membros.

## <a name="http-request"></a>Solicitação HTTP

### <a name="get-the-metadata-of-the-photo"></a>Obter os metadados da foto

Este ponto de extremidade retornará os metadados da foto. Se nenhum tamanho for especificado, os metadados para o maior tamanho de foto disponível serão retornados.

<!-- {
  "blockType": "ignored"
}-->

```http
GET /teams/{id}/photo
GET /teams/{id}/photo/{size}
```

### <a name="get-the-photo"></a>Obter a foto

Este ponto de extremidade recuperará os dados binários da foto. Se nenhum tamanho for especificado, o maior tamanho disponível será retornado.

<!-- {
  "blockType": "ignored"
}-->

```http
GET /beta/teams/{id}/photo/$value
GET /beta/teams/{id}/photo/{size}/$value
```

## <a name="path-parameters"></a>Parâmetros do caminho

Este método suporta um parâmetro de caminho opcional para especificar o tamanho da foto a ser recuperada. Você pode especificar qualquer tamanho até o maior tamanho disponível. Obtenha os metadados da foto para determinar o maior tamanho disponível.

|**Parâmetro**|**Tipo**|**Descrição**|
|:-----|:-----|:-----|
|size  |Cadeia de caracteres  | Um tamanho de foto. Os tamanhos suportados das fotos em HD do Microsoft 365 são os seguintes: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 e 648x648. As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory. Opcional.|

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor           |
|:--------------|:--------------  |
| Autorização | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo para esta solicitação.

## <a name="response"></a>Resposta

### <a name="response-for-getting-the-metadata-of-a-photo"></a>Resposta para obter os metadados de uma foto

Se bem-sucedido, esse método retornará um código de resposta `200 OK` e metadados sobre a foto.

### <a name="response-for-getting-the-photo"></a>Resposta para obter a foto

Se bem-sucedido, esse método retornará um código de resposta `200 OK` e os dados binários da foto.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-the-photo-metadata"></a>Exemplo 1: obter os metadados da foto

#### <a name="request"></a>Solicitação

Aqui está um exemplo da solicitação para obter os metadados da foto da equipe.

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo_metadata"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo
```

#### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ddfcd489-628b-7d04-b48b-20075df800e5')/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/teams('ddfcd489-628b-7d04-b48b-20075df800e5')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

### <a name="example-2-get-a-specific-size-of-the-team-photo"></a>Exemplo 2: obter um tamanho específico da foto da equipe

Aqui está um exemplo da solicitação para obter a foto da equipe em um tamanho específico.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo/240x240/$value
```

#### <a name="response"></a>Resposta

Contém os dados binários da foto 240x240 solicitada. O código de resposta HTTP é 200.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get team photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


