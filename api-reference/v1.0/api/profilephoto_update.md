<a id="update-profilephoto" class="xliff"></a>

# Atualizar profilephoto

Atualize a foto do **user** conectado, ou do **group** ou **contact** especificado. Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho da foto que você pode adicionar a 4 MB.

Você pode usar PATCH ou PUT para esta operação na versão 1.0.

> **Observação** Esta operação na versão 1.0 é compatível com caixas de correio corporativas ou de estudante ou caixas de correio não pessoais dos usuários


<a id="prerequisites" class="xliff"></a>

## Pré-requisitos
Um dos seguintes **escopos** é necessário para executar essa API para:

- Foto do perfil de **usuário** conectado  - *User.ReadWrite*, *User.ReadWrite.All*
- Foto do perfil de um **group**  -  *Group.ReadWrite.All*
- Foto de um **contact**  -  *Contacts.ReadWrite*

> **Observação:** para atualizar a foto de qualquer usuário na organização, o aplicativo deve ter a Permissão de aplicativo User.ReadWrite.All e chamar esta API usando a própria identidade, não em nome de um usuário. Para saber mais, veja como [obter acesso sem um usuário conectado](../../../concepts/auth_v2_service.md).

<a id="http-request-to-update-the-photo" class="xliff"></a>

## Solicitação HTTP para atualizar a foto
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/photo/$value
PATCH /users/{id | userPrincipalName}/photo/$value
PATCH /groups/{id}/photo/$value
PATCH /me/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PATCH /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value

PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
<a id="request-headers" class="xliff"></a>

## Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | image/jpeg. Obrigatório.  |

<a id="request-body" class="xliff"></a>

## Corpo da solicitação
Inclua os dados binários da foto no corpo da solicitação.

<a id="response" class="xliff"></a>

## Resposta
Se bem-sucedido, este método retorna um código de resposta `200 OK`.
<a id="example" class="xliff"></a>

## Exemplo
<a id="request" class="xliff"></a>

##### Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/v1.0/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
<a id="response" class="xliff"></a>

##### Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
