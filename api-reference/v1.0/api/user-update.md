---
title: Atualizar usuário
description: Atualize as propriedades de um objeto user.
author: jpettere
ms.localizationpriority: high
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 7da1279a39fd98e0284d875077a168bb4e5934c9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109651"
---
# <a name="update-user"></a>Atualizar usuário

Namespace: microsoft.graph

Atualizar as propriedades de um objeto [usuário](../resources/user.md). Nem todas as propriedades podem ser atualizadas por usuários Membros ou Convidados com suas permissões padrão sem Funções de administrador. [Compare as permissões padrão de membros e convidados](/azure/active-directory/fundamentals/users-default-permissions#compare-member-and-guest-default-permissions) para ver as propriedades que eles podem gerenciar.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | User.ReadWrite    |
|Aplicativo | User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All |

>[!NOTE]
> - Ao atualizar a propriedade **passwordProfile**, a seguinte permissão é necessária: Directory.AccessAsUser.All.
> - A atualização da propriedade **businessPhones**, **mobilePhone** ou **otherMails** de outro usuário é permitida apenas em usuários que não sejam administradores ou que tenham uma das seguintes funções: Leitor de Diretório, Emissor de Convites Independente, Leitor do Centro de Mensagens e Leitor de Relatórios. Para obter mais detalhes, confira Administrador de suporte técnico (senha) em [funções internas do Azure Active Directory](/azure/active-directory/roles/permissions-reference).  Esse é o caso de aplicativos que receberam as permissões User.ReadWrite.All ou Directory.ReadWrite.All delegadas ou de aplicativo.
> - Sua conta Microsoft pessoal deve estar vinculada a um locatário do AAD para atualizar seu perfil com a permissão delegada User.ReadWrite em uma conta Microsoft pessoal.
> - A atualização da propriedade **Identidades** exige a permissão User.ManageIdentities.All. Além disso, não é permitido adicionar uma [conta local B2C](../resources/objectidentity.md) a um objeto de **usuário** existente, a menos que o objeto de **usuário** já tenha uma identidade de conta local.

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
|aboutMe|String|Um campo de entrada de texto em forma livre para o usuário se descrever.|
|accountEnabled|Booliano| `true` se a conta estiver habilitada; caso contrário, `false`. Essa propriedade é obrigatória quando um usuário é criado.    |
| ageGroup | [ageGroup](../resources/user.md#agegroup-values) | Define a faixa etária do usuário. Valores permitidos: `null`, `minor`, `notAdult` e `adult`. Confira as [definições de propriedades da faixa etária legal](../resources/user.md#legal-age-group-property-definitions) para obter mais informações. |
|birthday|DateTimeOffset|O aniversário do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|businessPhones| String collection | Números de telefone para o usuário. OBSERVAÇÃO: Embora isso seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.|
|city|String|A cidade em que o usuário está localizado.|
| companyName | String | O nome da empresa em que o usuário está associado. Essa propriedade pode ser útil para descrever a empresa de onde procede um usuário externo. O comprimento máximo do nome da empresa é 64 caracteres. |
| consentProvidedForMinor | [consentProvidedForMinor](../resources/user.md#consentprovidedforminor-values) | Define se o consentimento foi obtido para menores. Valores permitidos: `null`, `granted`, `denied` e `notRequired`. Confira as [definições de propriedades da faixa etária legal](../resources/user.md#legal-age-group-property-definitions) para obter mais informações. |
|country|Cadeia de caracteres|O país/região em que o usuário está localizado; por exemplo, `US` ou `UK`.|
|department|String|O nome do departamento no qual o usuário trabalha.|
|displayName|String|O nome exibido no catálogo de endereços do usuário. É geralmente a combinação do nome, da inicial do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. |
| employeeId | String | O identificador de funcionário atribuído ao usuário pela organização. |
| employeeType | String | Captura o tipo de trabalhador corporativo. Por exemplo, `Employee`, `Contractor`, `Consultant` ou `Vendor`. Retornado apenas em `$select`.|
|givenName|String|O nome fornecido (nome) do usuário.|
|hireDate|DateTimeOffset|A data de contratação do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|interests|Coleção de cadeias de caracteres|Uma lista para o usuário descrever os interesses dele.|
|jobTitle|String|O cargo do usuário.|
|email|String|O endereço SMTP do usuário, por exemplo, `jeff@contoso.onmicrosoft.com`. As alterações feitas nessa propriedade também atualizarão a coleção **proxyAddresses** do usuário para incluir o valor como um endereço SMTP. Para contas do Azure AD B2C, esta propriedade só pode ser atualizada até dez vezes com endereços SMTP exclusivos. |
|mailNickname|String|O alias de e-mail do usuário. Essa propriedade deve ser especificada quando um usuário é criado.|
|mobilePhone|String|O número de celular principal do usuário.|
|mySite|String|A URL do site pessoal do usuário.|
|officeLocation|String|A localização do escritório no local de trabalho do usuário.|
| onPremisesExtensionAttributes | [onPremisesExtensionAttributes](../resources/onpremisesextensionattributes.md) | Contém extensionAttributes 1-15 para o usuário. Observe que os atributos de extensão individuais não são selecionáveis nem filtráveis. Para um usuário do `onPremisesSyncEnabled`, a fonte de autoridade desse conjunto de propriedades é o local e é somente leitura. Esses atributos de extensão também são conhecidos como atributos personalizados do Exchange 1-15.|
|onPremisesImmutableId|String|Essa propriedade é usada para associar uma conta de usuário do Active Directory local com seu objeto de usuário do Azure AD. Esta propriedade deverá ser especificada ao criar uma nova conta de usuário no Graph se você estiver usando um domínio federado para a propriedade **userPrincipalName** (UPN) do usuário. **Importante:** Os caracteres **$** e **_** e não podem ser usados ao especificar essa propriedade.                            |
|otherMails|String |Uma lista de endereços de email adicional para o usuário; Por exemplo: `["bob@contoso.com", "Robert@fabrikam.com"]`.|
|passwordPolicies|String|Especifica as políticas de senha do usuário. Este valor é uma enumeração com um valor possível sendo `DisableStrongPassword`, que permite que senhas mais fracas do que a política padrão sejam especificadas. `DisablePasswordExpiration` também pode ser especificado. Os dois podem ser especificados juntos; por exemplo: `DisablePasswordExpiration, DisableStrongPassword`.|
|passwordProfile|[PasswordProfile](../resources/passwordprofile.md)|Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte. Isto não pode ser usado para usuários federados. O *Diretório.AccessAsUser.All* permissão é necessária para atualizar esta propriedade.|
|pastProjects|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar seus projetos anteriores.|
|postalCode|String|O código postal do endereço postal do usuário. O código postal é específico para o país/região do usuário. Nos Estados Unidos, esse atributo contém o CEP.|
|preferredLanguage|String|O idioma preferencial do usuário. Deve seguir o Código ISO 639-1; por exemplo `en-US`.|
|responsibilities|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar suas responsabilidades.|
|schools|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar as escolas que ele frequentou.|
|skills|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar suas qualificações.|
|state|String|O estado ou município no endereço do usuário.|
|streetAddress|String|O endereço do local de trabalho do usuário.|
|surname|String|O sobrenome do usuário (nome de família ou sobrenome).|
|usageLocation|String|Um código de duas letras (padrão ISO 3166). Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços nos países.  Os exemplos incluem:`US`,`JP` e `GB`. Não anulável.|
|userPrincipalName|String|O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** de [organization](../resources/organization.md).
|userType|String|Um valor de string que pode ser usado para classificar tipos de usuário em seu diretório, como `Member` e `Guest`.          |

> [!NOTE] 
> As propriedades a seguir não podem ser atualizadas usando um contexto somente de aplicativo: **aboutMe**, **birthday**, **hireDate**, **interests**, **mySite**, **pastProjects**, **preferredName**, **responsibilities**, **schools** e **skills**.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="example"></a>Exemplo

### <a name="example-1-update-properties-of-the-signed-in-user"></a>Exemplo 1: atualizar as propriedades do usuário conectado

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra uma solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me
Content-type: application/json

{
  "businessPhones": [
    "+1 425 555 0109"
  ],
  "officeLocation": "18/2111"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta
O exemplo a seguir mostra a resposta.
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a>Exemplo 2: atualizar as propriedades do usuário especificado

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra uma solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_other_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id}
Content-type: application/json

{
  "businessPhones": [
    "+1 425 555 0109"
  ],
  "officeLocation": "18/2111"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

O exemplo a seguir mostra a resposta.
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```


### <a name="example-3-update-the-passwordprofile-of-a-user-to-reset-their-password"></a>Exemplo 3: atualizar o passwordProfile de um usuário para redefinir sua senha

O exemplo a seguir mostra uma solicitação para redefinir a senha de outro usuário.

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user_passwordProfile"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id}
Content-type: application/json

{
  "passwordProfile": {
    "forceChangePasswordNextSignIn": false,
    "password": "xWwvJ]6NMw+bWH-d"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-passwordprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-passwordprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-passwordprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-passwordprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response"
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
