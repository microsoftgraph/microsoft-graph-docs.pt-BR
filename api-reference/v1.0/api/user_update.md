
# <a name="update-user"></a>Atualizar usuário

Atualize as propriedades de um objeto user.
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | User.ReadWrite    |
|Aplicativo | User.ReadWrite.All, Directory.ReadWrite.All |

Ao atualizar a propriedade passwordProfile, a seguinte permissão é necessária: Directory.AccessAsUser.All.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor|
|:-----------|:------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|aboutMe|Sequência de caracteres|Um campo de entrada de texto em forma livre para o usuário se descrever.|
|accountEnabled|Boolean| **true** se a conta estiver habilitada; caso contrário, **false**. Essa propriedade é obrigatória quando um usuário é criado. Oferece suporte a $filter.    |
|birthday|DateTimeOffset|O aniversário do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|city|Sequência de caracteres|A cidade em que o usuário está localizado. Oferece suporte a $filter.|
|country|Sequência de caracteres|País/região em que o usuário está localizado. Por exemplo, "EUA" ou "Reino Unido". Oferece suporte a $filter.|
|department|Sequência de caracteres|O nome do departamento no qual o usuário trabalha. Oferece suporte a $filter.|
|displayName|Sequência de caracteres|O nome exibido no catálogo de endereços do usuário. É geralmente a combinação do nome, da inicial do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.|
|givenName|Sequência de caracteres|O nome fornecido (nome) do usuário. Oferece suporte a $filter.|
|hireDate|DateTimeOffset|A data de contratação do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|interests|Coleção de cadeias de caracteres|Uma lista para o usuário descrever os interesses dele.|
|jobTitle|Sequência de caracteres|O cargo do usuário. Oferece suporte a $filter.|
|mailNickname|Sequência de caracteres|O alias de email do usuário. Essa propriedade deve ser especificada quando um usuário é criado. Oferece suporte a $filter.|
|mobilePhone|Sequência de caracteres|O número de celular principal do usuário.|
|mySite|Sequência de caracteres|A URL do site pessoal do usuário.|
|officeLocation|Sequência de caracteres|A localização do escritório no local de trabalho do usuário.|
|onPremisesImmutableId|Sequência de caracteres|Essa propriedade é usada para associar uma conta de usuário do Active Directory local com seu objeto de usuário do Azure AD. Essa propriedade deverá ser especificada ao criar uma nova conta de usuário no Graph se você estiver usando um domínio federado para a propriedade **userPrincipalName** (UPN) do usuário. **Importante:** Os caracteres **$** e **_** não podem ser usados ao especificar essa propriedade. Oferece suporte a $filter.                            |
|passwordPolicies|Sequência de caracteres|Especifica as políticas de senha do usuário. Esse valor é uma enumeração cujo um dos valores possíveis é "DisableStrongPassword", o que permite especificar senhas mais fracas do que a política padrão. Também é possível especificar "DisablePasswordExpiration". Ambos podem ser especificados juntos; por exemplo: "DisablePasswordExpiration, DisableStrongPassword".|
|passwordProfile|[PasswordProfile](../resources/passwordprofile.md)|Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte.|
|pastProjects|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar seus projetos anteriores.|
|postalCode|Sequência de caracteres|O código postal do endereço postal do usuário. O código postal é específico para o país/região do usuário. Nos Estados Unidos, esse atributo contém o CEP.|
|preferredLanguage|Sequência de caracteres|O idioma preferencial do usuário. Deve seguir o código ISO 639-1; por exemplo "en-US".|
|preferredName|Sequência de caracteres|O nome preferencial do usuário.|
|responsibilities|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar suas responsabilidades.|
|schools|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar as escolas que ele frequentou.|
|skills|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar suas qualificações.|
|state|Sequência de caracteres|O estado ou município no endereço do usuário. Oferece suporte a $filter.|
|streetAddress|Sequência de caracteres|O endereço do local de trabalho do usuário.|
|surname|Sequência de caracteres|O sobrenome do usuário (nome de família ou sobrenome). Oferece suporte a $filter.|
|usageLocation|Sequência de caracteres|Um código de duas letras (padrão ISO 3166). Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços nos países. Entre os exemplos temos: "US", "JP" e "GB". Não anulável. Oferece suporte a $filter.|
|userPrincipalName|Sequência de caracteres|O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** de [organization](../resources/organization.md). Oferece suporte a $filter e $orderby.
|userType|Sequência de caracteres|Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como “Member” e “Guest”. Oferece suporte a $filter.          |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value"
}
```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
