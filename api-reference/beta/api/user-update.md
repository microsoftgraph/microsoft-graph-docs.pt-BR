---
title: Atualizar usuário
description: Atualize as propriedades de um objeto user.
author: jpettere
ms.localizationpriority: medium
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: b2e6b94ca21a04389c6472e7fda884817823353f
ms.sourcegitcommit: 033e779ba738b61b03e2760f39554a2fd0ab65b4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2022
ms.locfileid: "66788805"
---
# <a name="update-user"></a>Atualizar usuário

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualizar as propriedades de um objeto [usuário](../resources/user.md). Nem todas as propriedades podem ser atualizadas por usuários Membros ou Convidados com suas permissões padrão sem Funções de administrador. [Compare as permissões padrão de membros e convidados](/azure/active-directory/fundamentals/users-default-permissions#compare-member-and-guest-default-permissions) para ver as propriedades que eles podem gerenciar.

## <a name="permissions"></a>Permissões
Uma das seguintes pefrmissions é necessária para chamar essa API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.ReadWrite, User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | User.ReadWrite    |
|Aplicativo | User.ReadWrite.All, User.ManageIdentities.All, Directory.ReadWrite.All |

>[!NOTE]
> - A atualização da propriedade **businessPhones**, **mobilePhone** ou **otherMails** de outro usuário é permitida apenas em usuários que não sejam administradores ou que tenham uma das seguintes funções: Leitor de Diretório, Emissor de Convites Independente, Leitor do Centro de Mensagens e Leitor de Relatórios. Para obter mais detalhes, confira Administrador de suporte técnico (senha) em [funções internas do Azure Active Directory](/azure/active-directory/roles/permissions-reference).  Esse é o caso de aplicativos que receberam as permissões User.ReadWrite.All ou Directory.ReadWrite.All delegadas ou de aplicativo. Apenas um Administrador Global atribuído à permissão Directory.AccessAsUser.All pode atualizar essas propriedades aos administradores mais privilegiados.
> - Sua conta Microsoft pessoal deve estar vinculada a um locatário do AAD para atualizar seu perfil com a permissão delegada User.ReadWrite em uma conta Microsoft pessoal.
> - A atualização da propriedade **Identidades** exige a permissão User.ManageIdentities.All. Além disso, adicionar uma [conta local B2C](../resources/objectidentity.md) a um objeto **usuário** existente não é permitido, a menos que o objeto **usuário** já contenha uma identidade de conta local.

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
|accountEnabled|Booliano| `true` se a conta estiver habilitada; caso contrário, `false`. Essa propriedade é obrigatória quando um usuário é criado. Um administrador global com a permissão delegada _Directory.AccessAsUser.All_ pode atualizar o status **accountEnabled** de todos os administradores no locatário.|
| ageGroup | [ageGroup](../resources/user.md#agegroup-values) | Define a faixa etária do usuário. Valores permitidos: `null`, `Minor`, `NotAdult` e `Adult`. Confira as [definições de propriedades da faixa etária legal](../resources/user.md#legal-age-group-property-definitions) para obter mais informações. |
|assignedLicenses|Coleção [assignedLicense](../resources/assignedlicense.md)|As licenças que são atribuídas ao usuário. Não anulável.            |
|birthday|DateTimeOffset|O aniversário do usuário. O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|businessPhones| String collection | Números de telefone para o usuário. **NOTA:** Embora esta seja uma coleção de cadeias de caracteres, apenas um número pode ser definido para essa propriedade.|
|city|String|A cidade em que o usuário está localizado.|
| CompanyName | String | O nome da empresa em que o usuário está associado. Essa propriedade pode ser útil para descrever a empresa de onde procede um usuário externo. O tamanho máximo é de 64 caracteres. |
| consentProvidedForMinor | [consentProvidedForMinor](../resources/user.md#consentprovidedforminor-values) | Define se o consentimento foi obtido para menores. Valores permitidos: `null`, `Granted`, `Denied` e `NotRequired`. Confira as [definições de propriedades da faixa etária legal](../resources/user.md#legal-age-group-property-definitions) para obter mais informações. |
|country|Cadeia de caracteres|O país/região em que o usuário está localizado; por exemplo, `US` ou `UK`.|
|customSecurityAttributes|[customSecurityAttributeValue](../resources/customsecurityattributevalue.md)|Um tipo complexo aberto que contém o valor de um atributo de segurança personalizado atribuído a um objeto de diretório.<br/><br/>Para atualizar este imóvel, o responsável pela chamada deve ser designado como Administrador de Atribuição de Atributos e deve receber a permissão *CustomSecAttributeAssignment.ReadWrite.All*.|
|department|String|O nome do departamento no qual o usuário trabalha.|
|displayName|String|O nome exibido no catálogo de endereços do usuário. É geralmente a combinação do nome, da inicial do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações.|
|employeeId|String|O identificador de funcionário atribuído ao usuário pela organização. O comprimento máximo é de 16 caracteres.|
| employeeType | String | Captura o tipo de trabalhador corporativo. Por exemplo, `Employee`, `Contractor`, `Consultant` ou `Vendor`.|
|givenName|String|O nome fornecido (nome) do usuário.|
|employeeHireDate|DateTimeOffset|A data de contratação do usuário. O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z` |
|Identidades|Coleção [objectIdentity](../resources/objectidentity.md)| Representa as identidades que podem ser usadas para entrar nesta conta de usuário. Uma identidade pode ser fornecida pela Microsoft, por organizações ou por provedores de identidade social, como o Facebook, Google e Microsoft, e está vinculada a uma conta de usuário. Qualquer atualização de **identidades** substituirá toda a coleção e você deverá fornecer a identidade userPrincipalName **signInType** na coleção.|
|interests|Coleção de cadeias de caracteres|Uma lista para o usuário descrever os interesses dele.|
|jobTitle|String|O cargo do usuário.|
|email|String|O endereço SMTP do usuário, por exemplo, `jeff@contoso.onmicrosoft.com`. Para contas do Azure AD B2C, esta propriedade só pode ser atualizada até dez vezes com endereços SMTP exclusivos. As alterações feitas nessa propriedade também atualizarão a coleção **proxyAddresses** do usuário para incluir o valor como um endereço SMTP.|
|mailNickname|String|O alias de e-mail do usuário. Essa propriedade deve ser especificada quando um usuário é criado.|
|mobilePhone|String|O número de celular principal do usuário.|
|mySite|String|A URL do site pessoal do usuário.|
|officeLocation|String|A localização do escritório no local de trabalho do usuário.|
| onPremisesExtensionAttributes | [onPremisesExtensionAttributes](../resources/onpremisesextensionattributes.md) | Contém extensionAttributes 1-15 para o usuário. Observe que os atributos de extensão individuais não são selecionáveis nem filtráveis. Para um usuário do `onPremisesSyncEnabled`, a fonte de autoridade desse conjunto de propriedades é o local e é somente leitura. Esses atributos de extensão também são conhecidos como atributos personalizados do Exchange 1-15.|
|onPremisesImmutableId|String|Essa propriedade é usada para associar uma conta de usuário do Active Directory local com seu objeto de usuário do Azure AD. Esta propriedade deverá ser especificada ao criar uma nova conta de usuário no Graph se você estiver usando um domínio federado para a propriedade **userPrincipalName** (UPN) do usuário. **Importante:** Os caracteres **$** e **_** não podem ser usados ao especificar essa propriedade.                            |
|otherMails|Coleção String|Uma lista de endereços de email adicional para o usuário; Por exemplo: `["bob@contoso.com", "Robert@fabrikam.com"]`.|
|passwordPolicies|String|Especifica as políticas de senha do usuário. Esse valor é uma enumeração cujo um dos valores possíveis é `DisableStrongPassword`, o que permite especificar senhas mais fracas do que a política padrão. Também é possível especificar `DisablePasswordExpiration`. Ambos podem ser especificados juntos; por exemplo: `DisablePasswordExpiration, DisableStrongPassword`.|
|passwordProfile|[PasswordProfile](../resources/passwordprofile.md)|Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte.<br><br> No acesso delegado, o aplicativo de chamada deve receber a permissão delegada *Directory.AccessAsUser.All* em nome do usuário conectado. No acesso somente do aplicativo, o aplicativo de chamada deve receber a permissão *de aplicativo User.ReadWrite.All* e, pelo menos, a função user *administrator* [Azure AD.](/azure/active-directory/roles/permissions-reference)|
|pastProjects|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar seus projetos anteriores.|
|postalCode|String|O código postal do endereço postal do usuário. O código postal é específico para o país/região do usuário. Nos Estados Unidos, esse atributo contém o CEP.|
|preferredLanguage|Cadeia de caracteres|O idioma preferencial do usuário. Deve seguir o Código ISO 639-1; por exemplo, `en-US`.|
|responsibilities|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar suas responsabilidades.|
|schools|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar as escolas que ele frequentou.|
|skills|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar suas qualificações.|
|state|String|O estado ou município no endereço do usuário.|
|streetAddress|String|O endereço do local de trabalho do usuário.|
|surname|String|O sobrenome do usuário (nome de família ou sobrenome).|
|usageLocation|String|Um código de duas letras (padrão ISO 3166). Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços nos países/regiões. Por exemplo: `US`, `JP`, e `GB`. Não anulável.|
|userPrincipalName|Cadeia de caracteres|O nome UPN do usuário. O UPN é uma ID de logon do usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Os domínios verificados do locatário podem ser acessados pela propriedade **verifiedDomains** da [organização](../resources/organization.md).<br>OBSERVAÇÃO: esta propriedade não pode conter caracteres de ênfase. Somente os seguintes caracteres são permitidos `A - Z`, `a - z`, `0 - 9`, ` ' . - _ ! # ^ ~`. Para obter a lista completa de caracteres permitidos, consulte as [políticas de nome de usuário](/azure/active-directory/authentication/concept-sspr-policy#userprincipalname-policies-that-apply-to-all-user-accounts).|
|userType|String|Um valor de string que pode ser usado para classificar tipos de usuário em seu diretório, como `Member` e `Guest`.          |

Como o **recurso** de usuário dá suporte a extensões, `PATCH` você pode usar a operação para adicionar, atualizar ou excluir seus próprios dados [específicos](/graph/extensibility-overview) do aplicativo em propriedades personalizadas de uma extensão em uma instância de **usuário existente.**

> [!NOTE] 
> - As propriedades a seguir não podem ser atualizadas por um aplicativo com apenas permissões de aplicativo: **aboutMe**, **birthday**, **employeeHireDate**, **interests**, **mySite**, **pastProjects**, **responsabilidades**, **escolas** e **habilidades**.
> - Para atualizar as propriedades a seguir, você deve especificá-las em sua própria solicitação PATCH, sem incluir as outras propriedades listadas na tabela acima: **aboutMe**, **birthday**, **interests**, **mySite**, **pastProjects**, **responsabilidades**, **escolas** e **habilidades**.

### <a name="manage-extensions-and-associated-data"></a>Gerenciar extensões e dados associados

Use essa API para gerenciar o diretório, o esquema e as extensões abertas e seus dados para os usuários, da seguinte maneira:

+ Adicionar, atualizar e armazenar dados nas extensões de um usuário existente
+ Para extensões de diretório e esquema, remova todos os dados armazenados definindo o valor da propriedade de extensão personalizada como `null`. Para extensões abertas, use a API [Excluir a extensão aberta](/graph/api/opentypeextension-delete).

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
PATCH https://graph.microsoft.com/beta/me
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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-user-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-user-powershell-snippets.md)]
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
PATCH https://graph.microsoft.com/beta/users/{id}
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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-other-user-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-other-user-powershell-snippets.md)]
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

O exemplo a seguir mostra uma solicitação que redefine a senha de outro usuário.

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user_passwordProfile"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-user-passwordprofile-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-user-passwordprofile-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-4-assign-a-custom-security-attribute-with-a-string-value-to-a-user"></a>Exemplo 4: Atribuir um atributo de segurança personalizado com um valor de cadeia de caracteres a um usuário

O exemplo a seguir mostra como atribuir um atributo de segurança personalizado com um valor de cadeia de caracteres a um usuário.

+ Conjunto de atributos: `Engineering`
+ Atributo: `ProjectDate`
+ Tipo de dados de atributo: cadeia de caracteres
+ Valor do atributo: `"2022-10-01"`

Para atribuir atributos de segurança personalizados, o principal de chamada deve ser atribuído à função de Administrador de Atribuição de Atributo e deve receber a permissão *CustomSecAttributeAssignment.ReadWrite.All*.

Para obter mais exemplos para usuários, consulte [Atribuir, atualizar ou remover atributos de segurança personalizados usando o Microsoft API do Graph](/graph/custom-security-attributes-examples).

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "assign_user_customsecurityattribute_string"
}-->
```http
PATCH https://graph.microsoft.com/beta/users/{id}
Content-type: application/json

{
    "customSecurityAttributes":
    {
        "Engineering":
        {
            "@odata.type":"#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
            "ProjectDate":"2022-10-01"
        }
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/assign-user-customsecurityattribute-string-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/assign-user-customsecurityattribute-string-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/snippet-unavailable.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/snippet-unavailable.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/assign-user-customsecurityattribute-string-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/assign-user-customsecurityattribute-string-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-5-add-or-update-the-values-of-a-schema-extension-for-a-user"></a>Exemplo 5: Adicionar ou atualizar os valores de uma extensão de esquema para um usuário

Você pode atualizar ou atribuir um valor a uma única propriedade ou a todas as propriedades na extensão.

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/beta/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e
Content-type: application/json

{
    "ext55gb1l09_msLearnCourses": {
        "courseType": "Admin"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-schemaextension-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-schemaextension-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

>**Observação:** Para remover o valor da extensão do esquema do objeto do usuário, defina a propriedade como `null`. Por exemplo:
>
>```http
>PATCH https://graph.microsoft.com/v1.0/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e
>Content-type: application/json
>
>{
>    "ext55gb1l09_msLearnCourses": null
>}
>```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas (visualização)](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando extensões do esquema (visualização)](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
