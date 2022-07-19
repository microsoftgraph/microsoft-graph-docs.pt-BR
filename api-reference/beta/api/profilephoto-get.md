---
title: Get profilePhoto
description: Obtém o profilePhoto especificado ou seus metadados (propriedades profilePhoto).
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: people
author: kevinbellinger
ms.openlocfilehash: cc86e6dfc1e2aeb57c65d00f383c90842f30e2cb
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66855622"
---
# <a name="get-profilephoto"></a>Get profilePhoto

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha a [Foto do perfil especificado](../resources/profilephoto.md) ou seus metadados (propriedades da **Foto do perfil**) no Microsoft 365.

> **Nota**: ao tentar OBTER uma foto de **usuário**, esta operação primeiro tenta recuperar a foto especificada no Microsoft 365. Se a foto não estiver disponível no Microsoft 365, a API tentará recuperar a foto do Azure Active Directory.

Os tamanhos suportados de fotos em HD no Microsoft 365 são os seguintes: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 e 648x648. As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.

Você pode obter os metadados da maior foto disponível ou especificar um tamanho para obter os metadados do tamanho dessa foto.
Se o tamanho solicitado não estiver disponível, você ainda poderá obter um tamanho menor que o usuário carregou e disponibilizou.
Por exemplo, quando o usuário carrega uma foto de 504x504 pixels, todos os tamanhos de foto ficam disponíveis para baixar, exceto o de 648x648.
Caso o tamanho especificado não esteja disponível na caixa de correio do usuário ou no Azure Active Directory, o tamanho 1x1 será retornado com o restante dos metadados.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

> **Observação:** o método OBTER foto em beta tem suporte para contas corporativas, de estudante ou pessoais do usuário. O método OBTER foto metadados, no entanto, tem suporte apenas para contas corporativas ou de estudante do usuário, ficando de fora as contas pessoais.

### <a name="to-retrieve-the-profile-photo-of-a-contact"></a>Para recuperar a foto do perfil de um contato

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)      |   Contacts.Read, Contacts.ReadWrite           |
|Delegado (conta pessoal da Microsoft)      |   Contacts.Read, Contacts.ReadWrite            |
|Aplicativo      |    Contacts.Read, Contacts.ReadWrite           |

### <a name="to-retrieve-the-profile-photo-of-a-group"></a>Para recuperar a foto do perfil de um grupo

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)      |   Group.Read.All, Group.ReadWrite.All           |
|Delegado (conta pessoal da Microsoft)      |   Sem suporte.            |
|Aplicativo      |    Group.Read.All, Group.ReadWrite.All           |

### <a name="to-retrieve-the-profile-photo-of-a-team"></a>Para recuperar a foto de perfil de uma equipe

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All **, Group.ReadWrite.All**, Directory.Read.All **, Directory.ReadWrite.All** |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Application | TeamSettings.Read.Group *, TeamSettings.ReadWrite.Group*, Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All **, Group.ReadWrite.All**, Directory.Read.All **, Directory.ReadWrite.All**  |

### <a name="to-retrieve-the-profile-photo-of-a-user"></a>Para recuperar a foto do perfil de um usuário

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)      |   User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All           |
|Delegado (conta pessoal da Microsoft)      |   User.Read, User.ReadWrite            |
|Aplicativo      |    User.Read.All, User.ReadWrite.All           |



> [!NOTE]
> 
> 1. Não há suporte para a operação de metadados em contas pessoais da Microsoft.
> 2. Atualmente, há um [problema conhecido](/graph/known-issues#groups) ao acessar fotos de grupo usando permissões de aplicativos.
> 3. Atualmente, não há suporte para a recuperação da foto de um usuário usando o Microsoft API do Graph em locatários Azure AD B2C.

## <a name="http-request"></a>Solicitação HTTP

### <a name="get-the-photo"></a>Obter a foto
<!-- { "blockType": "ignored" } -->

```http
GET /me/photo/$value
GET /users/{id | userPrincipalName}/photo/$value
GET /groups/{id}/photo/$value
GET /me/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contacts/{id}/photo/$value
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
GET /team/{id}/photo/$value
```

### <a name="get-the-metadata-of-the-photo"></a>Obter os metadados da foto
<!-- { "blockType": "ignored" } -->

```http
GET /me/photo
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /me/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contacts/{id}/photo
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo
GET /team/{id}/photo
```

### <a name="get-the-metadata-for-a-specific-photo-size"></a>Obter os metadados de um tamanho de página específica.
<!-- { "blockType": "ignored" } -->

```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
```

## <a name="path-parameters"></a>Parâmetros do caminho

|**Parâmetro**|**Tipo**|**Descrição**|
|:-----|:-----|:-----|
|size  |Cadeia de caracteres  | Um tamanho de foto. Os tamanhos suportados das fotos em HD do Microsoft 365 são os seguintes: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 e 648x648. As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory. |

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
### <a name="response-for-getting-the-photo"></a>Resposta para obter a foto
Se for bem-sucedido, este método retornará um código de resposta `200 OK` e dados binários da foto solicitada.  Se não existirem fotos, a operação retornará `404 Not Found`.
### <a name="response-for-getting-the-metadata-of-the-photo"></a>Resposta para obter os metadados da foto
Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [profilePhoto](../resources/profilephoto.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-the-photo-of-the-signed-in-user-in-the-largest-available-size"></a>Exemplo 1: Obtenha a foto do usuário conectado no maior tamanho disponível

##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "ignored"
}-->

```http
GET https://graph.microsoft.com/beta/me/photo/$value
Content-Type: image/jpg
```

##### <a name="response"></a>Resposta
Contém os dados binários da foto solicitada. O código de resposta HTTP é 200.

### <a name="example-2-get-the-48x48-photo-for-the-signed-in-user"></a>Exemplo 2: Obtenha foto 48 x 48 para usuário conectado

##### <a name="request"></a>Solicitação
<!-- {
  "blockType": "ignored"
}-->

```http
GET https://graph.microsoft.com/beta/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response"></a>Resposta
Contém os dados binários da foto 48x48 solicitada. O código de resposta HTTP é 200.

### <a name="example-3-get-the-metadata-of-the-user-photo-of-the-signed-in-user"></a>Exemplo 3: Esta solicitação obtém os metadados da foto do usuário conectado.

##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "ignored"
}-->

```http
GET https://graph.microsoft.com/beta/me/photo
```

##### <a name="response"></a>Resposta
Os dados de resposta a seguir mostram os metadados da foto.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "ignored"
}-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240x240",
    "width": 240,
    "height": 240
}
```

Os dados de resposta a seguir mostram o conteúdo de uma resposta quando uma foto ainda não foi carregada para o usuário.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "ignored"
}-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/gif",
    "@odata.mediaEtag": "",
    "id": "1x1",
    "width": 1,
    "height": 1
}
```

### <a name="example-4-get-the-photo-metadata"></a>Exemplo 4: Obter os metadados da foto

#### <a name="request"></a>Solicitação

Aqui está um exemplo da solicitação para obter os metadados da foto da equipe.

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo_metadata"
}-->
```http
GET https://graph.microsoft.com/beta/teams/172b0cce-e65d-44ce-9a49-91d9f2e8491e/photo
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('172b0cce-e65d-44ce-9a49-91d9f2e8491e')/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/teams('172b0cce-e65d-44ce-9a49-91d9f2e8491e')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

### <a name="example-5-get-the-team-photos-binary-data"></a>Exemplo 5: Obter os dados binários da foto da equipe

Aqui está um exemplo da solicitação para obter os dados binários da foto da equipe.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo"
}-->
```http
GET https://graph.microsoft.com/beta/teams/172b0cce-e65d-44ce-9a49-91d9f2e8491e/photo/$value
```

#### <a name="response"></a>Resposta

Contém os dados binários da foto solicitada. O código de resposta HTTP é 200.

## <a name="using-the-binary-data-of-the-requested-photo"></a>Usando os dados binários da foto solicitada

Ao usar o ponto de extremidade `/photo/$value` para obter os dados binários de uma foto de perfil, você precisa converter os dados em uma cadeia de caracteres da base 64 para adicioná-la como um anexo de email. Veja aqui um exemplo no JavaScript de como criar uma matriz que você pode passar como o valor do parâmetro `Attachments` de uma [Mensagem do Outlook](user-post-messages.md).

```javascript
const attachments = [{
  '@odata.type': '#microsoft.graph.fileAttachment',
  ContentBytes: file.toString('base64'),
  Name: 'mypic.jpg'
}];
```

Confira [Amostra de conexão do Microsoft Graph para Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) para ver uma implementação desse exemplo.

Se você quiser exibir a imagem em uma página da Web, crie um objeto na memória com base na imagem e torne esse objeto a origem de um elemento de imagem. Eis um exemplo em JavaScript dessa operação.

```javascript
const url = window.URL || window.webkitURL;
const blobUrl = url.createObjectURL(image.data);
document.getElementById(imageElement).setAttribute("src", blobUrl);
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


