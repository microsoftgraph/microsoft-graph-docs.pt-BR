# <a name="section-copytosectiongroup"></a>section: copyToSectionGroup
Copia uma seção para um grupo de seção específico.

Para operações Copiar, siga um padrão de chamada assíncrono:  Primeiro, chame a ação Copiar e, em seguida, sonde o ponto de extremidade da operação para ver o resultado.

## <a name="prerequisites"></a>Pré-requisitos
Um dos seguintes **escopos** é obrigatório para executar esta API:   

Notes.Create, Notes.ReadWrite ou Notes.ReadWrite.All 

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Autorização  | string  | `Bearer <token>` Um token OAuth válido fornecido para o aplicativo com base nas credenciais do usuário e o usuário ter acesso autorizado. |
| Content-Type | string | `application/json` |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça um objeto JSON que contém os parâmetros que a operação precisa.

| Parâmetro       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|groupId|String|A id do grupo para o qual copiar. Use somente quando copiar para um grupo do Office 365.|
|id|String|Obrigatório. A id do grupo de seção de destino. |
|renameAs|String|O nome da cópia. Restabelece o padrão do nome do item existente. |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a>Resposta
Se bem-sucedido, esse método retornará um código de resposta `202 Accepted` e um cabeçalho `Operation-Location`. Sonde o ponto de extremidade Operation-Location para [obter o status da operação de cópia](onenoteoperation_get.md).

## <a name="example"></a>Exemplo
Eis um exemplo de como chamar esta API.
##### <a name="request"></a>Solicitação
Veja a seguir um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->