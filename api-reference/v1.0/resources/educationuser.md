# <a name="educationuser-resource-type"></a>Tipo de recurso educationUser

Um usuário no sistema. Essa é uma variante específica de educação do usuário com a mesma `id` que o Microsoft Graph retornará do ponto de extremidade `/users` não específico da educação.
Esse objeto fornece um subconjunto direcionado de propriedades do objeto principal [user](user.md) e adiciona um conjunto de propriedades específico de educação, como dados de `primaryRole`, aluno e professor.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter educationUser](../api/educationuser_get.md) | [educationUser](educationuser.md) |Leia as propriedades e relações de um objeto **educationUser**.|
|[Listar classes](../api/educationuser_list_classes.md) |Coleção [educationClass](educationclass.md)| Obtenha a coleção de objetos **educationClass** da qual o usuário é membro.|
|[Listar escolas](../api/educationuser_list_schools.md) |Coleção [educationSchool](educationschool.md)| Obtenha a coleção de objetos **educationSchool** da qual o usuário é um membro.|
|[Obter usuário](../api/educationuser_get_user.md) |[user](user.md)| Obtenha o **user** do diretório simples que corresponde a esse **educationUser**.|
|[Atualizar](../api/educationuser_update.md) | [educationUser](educationuser.md)   |Atualize um objeto **educationUser**. |
|[Excluir](../api/educationuser_delete.md) | Nenhum |Exclua um objeto **educationUser**. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|accountEnabled|Booliano| **True** se a conta estiver habilitada; caso contrário, **false**. Essa propriedade é obrigatória quando um usuário é criado. Oferece suporte a $filter.    |
|assignedLicenses|Coleção [assignedLicense](assignedlicense.md)|As licenças que são atribuídas ao usuário. Não anulável.            |
|assignedPlans|Coleção [assignedPlan](assignedplan.md)|Os planos que são atribuídos ao usuário. Somente leitura. Não anulável. |
|businessPhones|Coleção de cadeias de caracteres|Números de telefone para o usuário. **Observação:** embora essa seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.|
|createdBy|[identitySet](identityset.md)| Entidade que criou o usuário. |
|department|String|O nome do departamento no qual o usuário trabalha. Oferece suporte a $filter.|
|displayName|String|O nome exibido para o usuário no catálogo de endereços. Geralmente é a combinação do nome, da inicial do nome do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.|
|externalSource|`educationExternalSource`| De onde esse usuário foi criado. Os valores possíveis são: `sis`, `manual`, `unkownFutureValue`.|
|givenName|String|O nome fornecido (nome) do usuário. Oferece suporte a $filter.|
|id|String|O identificador exclusivo do usuário. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura.|
|mail|Cadeia de caracteres|O endereço SMTP do usuário, por exemplo, "jeff@contoso.onmicrosoft.com". Somente Leitura. Oferece suporte a $filter.|
|mailingAddress|[physicalAddress](physicaladdress.md)| Endereço de email do usuário.|
|mailNickname|String|O alias de email do usuário. Essa propriedade deve ser especificada quando um usuário é criado. Oferece suporte a $filter.|
|middleName| Cadeia de caracteres | O nome do meio do usuário.|
|mobilePhone|String|O número de celular principal do usuário.|
|passwordPolicies|String|Especifica as políticas de senha do usuário. Esse valor é uma enumeração cujo um dos valores possíveis é "DisableStrongPassword", o que permite especificar senhas mais fracas do que a política padrão. Também é possível especificar "DisablePasswordExpiration". Os dois podem ser especificados juntos, por exemplo: "DisablePasswordExpiration, DisableStrongPassword".|
|passwordProfile|[PasswordProfile](passwordprofile.md)|Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte.|
|preferredLanguage|String|O idioma preferencial do usuário. Deve seguir o código ISO 639-1; por exemplo, "en-US".|
|primaryRole|cadeia de caracteres| Função padrão de um usuário. A função do usuário pode ser diferente em uma aula individual. Os valores possíveis são: `student`, `teacher`, `enum_sentinel`. Oferece suporte a $filter.|
|provisionedPlans|Coleção [ProvisionedPlan](provisionedplan.md)|Os planos que estão provisionados para o usuário. Somente leitura. Não anulável. |
|residenceAddress|[physicalAddress](physicaladdress.md)| Endereço em que o usuário reside.|
|student|[educationStudent](educationstudent.md)| Se a função principal for aluno, esse bloco conterá dados específicos do aluno.|
|surname|String|O sobrenome (nome de família) do usuário. Oferece suporte a $filter.|
|teacher|[educationTeacher](educationteacher.md)| Se a função principal for professor, esse bloco conterá dados específicos do professor.|
|usageLocation|Cadeia de caracteres|Um código de país de duas letras (padrão ISO 3166). Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços em países ou regiões. Os exemplos incluem: "US", "JP" e "GB". Não anulável. Oferece suporte a $filter.|
|userPrincipalName|String|O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** de [organization](organization.md). Oferece suporte a $filter e $orderby.
|userType|String|Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como “Member” e “Guest”. Oferece suporte a $filter.          |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|classes|Coleção [educationClass](educationclass.md)| Aulas às quais o usuário pertence. Anulável.|
|schools|Coleção [educationSchool](educationschool.md)| Escolas às quais o usuário pertence. Anulável.|
|assignments| [educationAssignment](../../beta/resources/educationAssignment.md)| Lista de atribuições do usuário. Anulável.|

>**Observação:** o recurso **educationassignment** é uma versão /beta. Se for usar esse recurso, não se esqueça de revisar o [log de alterações](../../../concepts/changelog.md) periodicamente. Quando os recursos de API do Microsoft Graph forem lançados no ponto de extremidade /v1.0, o lançamento será anotado no log de alterações. Se o aplicativo consumir o recurso **educationassignment**, será necessário declarar as URLs de solicitação básicas, como mostrado no seguinte bloco de códigos:  
```JavaScript
var v1BaseUrl = “https://graph.microsoft.com/v1.0/education”;
var betaBaseUrl = “https://graph.microsoft.com/beta/education”;  // for administrativeUnit and educationOrganization
```


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationUser"
}-->

```json
{
  "id": "string",
  "displayName": "string",
  "givenName": "string",
  "middleName": "string",
  "surname": "string",
  "mail": "string",
  "mobilePhone": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalSource": "string",
  "mailingAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "primaryRole": "string",
  "residenceAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "student": {"@odata.type": "microsoft.graph.educationStudent"},
  "teacher": {"@odata.type": "microsoft.graph.educationTeacher"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
