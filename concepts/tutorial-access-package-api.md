---
title: 'Tutorial: Gerenciar o acesso a recursos no gerenciamento de direitos do Active Directory usando as APIs do Microsoft Graph'
description: Saiba como gerenciar o acesso a recursos no gerenciamento de direitos do Active Directory (Azure AD) usando as APIs do Microsoft Graph.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ae9dfec7ae5db453ff6962ffd5684dd3bd9ee7d1
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271859"
---
# <a name="tutorial-manage-access-to-resources-in-active-directory-entitlement-management-using-microsoft-graph-apis"></a>Tutorial: Gerenciar o acesso a recursos no gerenciamento de direitos do Active Directory usando as APIs do Microsoft Graph

Gerenciar o acesso a todos os recursos de que os funcionários precisam, como grupos, aplicativos e sites, é uma função importante para as organizações. Você deseja conceder aos funcionários o nível certo de acesso que eles precisam para serem produtivos e remover o acesso quando não for mais necessário. O gerenciamento de direitos do [Azure Active Directory (Azure AD)](/azure/active-directory/governance/entitlement-management-overview) usando AS APIs do Microsoft Graph permite gerenciar esse tipo de acesso.

Neste tutorial, você foi solicitado a desenvolver código para criar um pacote de recursos para uma campanha de marketing que os usuários internos podem solicitar por autoatendigo. As solicitações não exigem aprovação e o acesso do usuário expira após 30 dias. Para este tutorial, os recursos da campanha de marketing são apenas membros de um único grupo, mas pode ser um conjunto de grupos, aplicativos ou sites do SharePoint Online.

>**Observação:** Os objetos de resposta mostrados neste tutorial podem ser reduzidos para maior leitura. 

## <a name="prerequisites"></a>Pré-requisitos

Para concluir com êxito este tutorial, certifique-se de que você tem os pré-requisitos necessários:
- O gerenciamento de direitos do Azure AD requer licenças específicas. Para obter mais informações, consulte [Requisitos de licença.](/azure/active-directory/governance/entitlement-management-overview#license-requirements) As seguintes licenças são necessárias em seu locatário:
    - Azure AD Premium P2
    - Licença enterprise Mobility + Security (EMS) E5
- Este tutorial assume que você está usando o Microsoft Graph Explorer, mas você pode usar o Postman ou criar seu próprio aplicativo cliente para chamar o Microsoft Graph. Para chamar as APIs do Microsoft Graph neste tutorial, você precisa usar uma conta com a função de administrador global e as permissões apropriadas. Para este tutorial, as permissões , e `User.ReadWrite.All` `Group.ReadWrite.All` `EntitlementManagement.ReadWrite.All` delegadas são necessárias. Conclua as seguintes etapas para definir permissões no Microsoft Graph Explorer:
    1. Iniciar [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).
    2. Selecione **Entrar com a Microsoft** e entre usando uma conta de administrador global do Azure AD. Depois de entrar com êxito, você poderá ver os detalhes da conta de usuário no painel esquerdo.
    3. Selecione o ícone de configurações à direita dos detalhes da conta do usuário e selecione **Selecionar permissões.**

        ![Selecionar as permissões do Microsoft Graph](./images/tutorial-access-package-api/set-permissions.png)
        
    4. Role pela lista de permissões para as `Group` permissões, expanda **Grupo (2),** selecione a **permissão Group.ReadWrite.All.** Role mais para baixo a lista de permissões para as `User` permissões, expanda **Usuário (8)** e selecione a **permissão User.ReadWrite.All.**

        ![Pesquisar as permissões de usuário, grupo e direito](./images/tutorial-access-package-api/set-user-permission.png)
    
    5. Selecione **Consentimento** e, em **seguida, selecione Aceitar** para aceitar o consentimento das permissões. Você não precisa consentir em nome de sua organização para essas permissões.
    6. Pesquise as `EntitlementManagement` permissões, expanda **EntitlementManagement (2)**, selecione a permissão **Entitlement.ReadWrite.All** e selecione **Consent**. Como essa permissão requer consentimento do administrador e é necessária por uma conta de usuário que você cria neste tutorial, você deve selecionar Consentimento **em nome da sua organização.**

        ![Consentimento para a organização](./images/tutorial-access-package-api/consent-for-organization.png)

    7. Selecione **Aceitar** para aceitar o consentimento das permissões.

## <a name="step-1-create-a-user-account-and-a-group"></a>Etapa 1: Criar uma conta de usuário e um grupo

Nesta etapa, você cria um grupo chamado Recursos de **Marketing** no diretório que é o recurso de destino para o gerenciamento de direitos. Você também cria uma conta de usuário que está configurada como um solicitante interno.

### <a name="create-a-user-account"></a>Criar uma conta de usuário

Para este tutorial, você cria uma conta de usuário que é usada para solicitar acesso aos recursos no pacote de acesso. Ao fazer essas chamadas, mude para `contoso.onmicrosoft.com` o nome de domínio do seu locatário. Você pode encontrar informações de locatário na página de visão geral do Azure Active Directory. Grave o valor da **propriedade de id** que será usada posteriormente no tutorial.

#### <a name="request"></a>Solicitação

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled":true,
  "displayName":"Requestor1",
  "mailNickname":"Requestor1",
  "userPrincipalName":"Requestor1@contoso.onmicrosoft.com",
  "passwordProfile": {
    "forceChangePasswordNextSignIn":true,
    "password":"Contoso1234"
  }
}
```

#### <a name="response"></a>Resposta

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
  "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
  "deletedDateTime": null,
  "accountEnabled": true,
  "ageGroup": null,
  "businessPhones": [],
  "city": null,
  "createdDateTime": null,
  "creationType": null,
  "companyName": null,
  "consentProvidedForMinor": null,
  "country": null,
  "department": null,
  "displayName": "Requestor1",
  "employeeId": null,
  "faxNumber": null,
  "givenName": null,
  "imAddresses": [],
  "infoCatalogs": [],
  "isResourceAccount": null,
  "jobTitle": null,
  "legalAgeGroupClassification": null,
  "mail": null,
  "mailNickname": "Requestor1",
}
```

### <a name="create-a-group"></a>Criar um grupo

Neste tutorial, você cria um grupo chamado Recursos de **Marketing** que é o recurso de destino para o gerenciamento de direitos. Você pode usar um grupo existente se já tiver um. Grave o valor da **propriedade de ID** que será retornada para uso posteriormente neste tutorial. 

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json

{
  "description":"Marketing group",
  "displayName":"Marketing resources",
  "mailEnabled":false,
  "mailNickname":"markres",
  "securityEnabled":true
}
```

#### <a name="response"></a>Resposta

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
  "id": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
  "deletedDateTime": null,
  "classification": null,
  "createdDateTime": "2020-06-24T16:47:37Z",
  "createdByAppId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
  "description": "Marketing group",
  "displayName": "Marketing resources",
  "expirationDateTime": null,
  "groupTypes": [],
  "infoCatalogs": [],
  "isAssignableToRole": null,
  "mail": null,
  "mailEnabled": false,
  "mailNickname": "markres"
}
```

## <a name="step-2-add-resources-to-a-catalog-and-create-an-access-package"></a>Etapa 2: Adicionar recursos a um catálogo e criar um pacote de acesso

Um *pacote de acesso* é um pacote de recursos que uma equipe ou projeto precisa e é governado por políticas. Os pacotes de acesso são definidos em contêineres chamados catálogos. Os catálogos podem fazer referência a recursos, como grupos, aplicativos e sites, que são usados no pacote de acesso. Nesta etapa, você cria um pacote **de acesso** à Campanha de Marketing no catálogo Geral. Se você tiver um catálogo diferente, use seu nome na próxima seção.

### <a name="get-the-catalog-identifier"></a>Obter o identificador de catálogo

Para adicionar recursos ao catálogo, primeiro você deve obter o identificador dele. Se você estiver usando o catálogo Geral, execute a solicitação a seguir para obter seu identificador. Se você estiver usando umlog diferente, altere o valor do filtro na solicitação para o nome do seu catálogo. Grave o valor da **propriedade de id** que será retornada para uso posteriormente neste tutorial.

#### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs?$filter=(displayName eq 'General')
```

#### <a name="response"></a>Resposta

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageCatalogs",
  "value": [ 
    {
      "id": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
      "displayName": "General",
      "description": "Built-in catalog.",
      "catalogType": "ServiceDefault",
      "catalogStatus": "Published",
      "isExternallyVisible": true,
      "createdBy": "Azure AD",
      "createdDateTime": "2020-05-30T10:58:05.363Z",
      "modifiedBy": "Azure AD",
      "modifiedDateTime": "2020-05-30T10:58:05.363Z"
    }
  ]
}
```

A resposta deve conter apenas o catálogo cujo nome você forneceu na solicitação. Se não houver valores retornados, verifique se o nome do catálogo está correto antes de prosseguir.

### <a name="add-the-group-to-the-catalog"></a>Adicionar o grupo ao catálogo

Para adicionar o grupo que você criou ao catálogo, forneça os seguintes valores de propriedade:
- **catalogId** - **a id** do catálogo que você está usando
- **displayName** - o nome do grupo
- **description** - a descrição do grupo
- **originId** - **a id** do grupo que você criou

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
  "catalogId":"cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "requestType": "AdminAdd",
  "justification": "",
  "accessPackageResource": {
    "displayName": "Marketing resources",
    "description": "Marketing group",
    "resourceType": "AadGroup",
    "originId": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
    "originSystem": "AadGroup"
  }
}
```

#### <a name="response"></a>Resposta

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceRequests/$entity",
  "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "executeImmediately": false,
  "id": "44e521e0-fb6b-4d5e-a282-e7e68dc59493",
  "requestType": "AdminAdd",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "isValidationOnly": false,
  "expirationDateTime": null,
  "justification": ""
}
```

### <a name="get-catalog-resources"></a>Obter recursos de catálogo

Nas etapas posteriores deste tutorial, você precisará da **id** que foi atribuída ao recurso de grupo no catálogo. Esse identificador, que representa o grupo como um recurso no catálogo, é diferente do identificador do próprio grupo no Microsoft Graph. Isso porque um catálogo pode ter recursos que não são representados no Microsoft Graph.

Na solicitação, forneça **a id** do catálogo que você está usando. Registrar o valor da propriedade **de ID** para o recurso de catálogo de grupo.

#### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/cec5d6ab-c75d-47c0-9c1c-92e89f66e384/accessPackageResources?$filter=(displayName eq 'Marketing resources')
```

#### <a name="response"></a>Resposta

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageResources",
  "value": [
    {
      "id": "4a1e21c5-8a76-4578-acb1-641160e076e8",
      "displayName": "Marketing resources",
      "description": "Marketing group",
      "url": "https://account.activedirectory.windowsazure.com/r?tenantId=d3030981-8fb9-4919-9980-5580caeddd75#/manageMembership?objectType=Group&objectId=e93e24d1-2b65-4a6c-a1dd-654a12225487",
      "resourceType": "Security Group",
      "originId": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
      "originSystem": "AadGroup",
      "isPendingOnboarding": false,
      "addedBy": "admin@contoso.onmicrosoft.com",
      "addedOn": "2020-08-21T19:27:29.967Z"
    }
  ]
}
```

### <a name="get-resources-roles"></a>Obter funções de recursos

O pacote de acesso atribui usuários às funções de um recurso. A função típica de um grupo é a função de membro. Outros recursos, como sites e aplicativos do SharePoint Online, podem ter muitas funções. A função típica de um grupo usado em um pacote de acesso é a função de membro. Você precisará da função de membro ao adicionar uma função de recurso ao pacote de acesso posteriormente neste tutorial. 

Na solicitação, use a **id** do catálogo e a **id** do recurso de grupo no catálogo que você gravou para obter **a originId** da função de recurso Membro. Grave o valor da **propriedade originId** a ser usada posteriormente neste tutorial.

#### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/cec5d6ab-c75d-47c0-9c1c-92e89f66e384/accessPackageResourceRoles?$filter=(originSystem+eq+%27AadGroup%27+and+accessPackageResource/id+eq+%274a1e21c5-8a76-4578-acb1-641160e076e8%27+and+displayName+eq+%27Member%27)&$expand=accessPackageResource
```

#### <a name="response"></a>Resposta

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageCatalogs('ede67938-cda7-4127-a9ca-7c7bf86a19b7')/accessPackageResourceRoles(accessPackageResource())",
  "value": [
    {
      "id": "00000000-0000-0000-0000-000000000000",
      "displayName": "Member",
      "description": null,
      "originSystem": "AadGroup",
      "originId": "Member_e93e24d1-2b65-4a6c-a1dd-654a12225487",
      "accessPackageResource@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageCatalogs('cec5d6ab-c75d-47c0-9c1c-92e89f66e384')/accessPackageResourceRoles('00000000-0000-0000-0000-000000000000')/accessPackageResource/$entity",
      "accessPackageResource": {
        "id": "4a1e21c5-8a76-4578-acb1-641160e076e8",
        "displayName": "Marketing resources",
        "description": "Marketing group",
        "url": "https://account.activedirectory.windowsazure.com/r?tenantId=d3030981-8fb9-4919-9980-5580caeddd75#/manageMembership?objectType=Group&objectId=e93e24d1-2b65-4a6c-a1dd-654a12225487",
        "resourceType": "Security Group",
        "originId": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
        "originSystem": "AadGroup",
        "isPendingOnboarding": false,
        "addedBy": "admin@contoso.onmicrosoft.com",
        "addedOn": "2020-06-26T17:13:23.723Z",
        "accessPackageResourceScopes@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageCatalogs('cec5d6ab-c75d-47c0-9c1c-92e89f66e384')/accessPackageResourceRoles('00000000-0000-0000-0000-000000000000')/accessPackageResource/accessPackageResourceScopes",
        "accessPackageResourceScopes": []
      }
    }
  ]
}
```

Se bem-sucedido, um único valor é retornado, que representa a função membro desse grupo. Se nenhuma função for retornada, verifique os **valores de ID** do catálogo e o recurso do pacote de acesso.

### <a name="create-the-access-package"></a>Criar o pacote de acesso

Neste ponto, você tem um catálogo com um recurso de grupo e sabe que usará a função de recurso do membro do grupo no pacote de acesso. A próxima etapa é criar o pacote de acesso. Depois de ter o pacote de acesso, você pode adicionar a função de recurso a ele e criar uma política de como os usuários podem solicitar acesso a essa função de recurso. Use a **id do** catálogo que você gravou anteriormente para criar o pacote de acesso. Grave a **id** do pacote de acesso para usar mais adiante neste tutorial.

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
Content-type: application/json

{
  "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "displayName": "Marketing Campaign",
  "description": "Access to resources for the campaign"
}
```

#### <a name="response"></a>Resposta

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackages/$entity",
  "id": "88203d16-0e31-41d4-87b2-dd402f1435e9",
  "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "displayName": "Marketing Campaign",
  "description": "Access to resources for the campaign",
  "isHidden": false,
  "isRoleScopesVisible": false,
  "createdBy": "admin@contoso.onmicrosoft.com",
  "createdDateTime": "2020-08-21T19:45:33.2042281Z",
  "modifiedBy": "admin@contoso.onmicrosoft.com",
  "modifiedDateTime": "2020-08-21T19:45:33.2042281Z"
}
```

### <a name="add-a-resource-role-to-the-access-package"></a>Adicionar uma função de recurso ao pacote de acesso

Adicione a função Membro do recurso de grupo ao pacote de acesso. Na solicitação, forneça a **id** do pacote de acesso. No corpo da solicitação, forneça a **id** do recurso do catálogo de grupos para accessPackageResource e forneça a **originId** da função Membro que você gravou anteriormente.

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/88203d16-0e31-41d4-87b2-dd402f1435e9/accessPackageResourceRoleScopes
Content-type: application/json

{
  "accessPackageResourceRole": {
    "originId":"Member_e93e24d1-2b65-4a6c-a1dd-654a12225487",
    "displayName":"Member",
    "originSystem":"AadGroup",
    "accessPackageResource": {
      "id":"4a1e21c5-8a76-4578-acb1-641160e076e8","resourceType":"Security Group",  
      "originId":"e93e24d1-2b65-4a6c-a1dd-654a12225487","originSystem":"AadGroup"
    }
  },
  "accessPackageResourceScope": {
    "originId":"e93e24d1-2b65-4a6c-a1dd-654a12225487","originSystem":"AadGroup"
  }
}
```

#### <a name="response"></a>Resposta

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackages('88203d16-0e31-41d4-87b2-dd402f1435e9')/accessPackageResourceRoleScopes/$entity",
  "id": "e081321b-2802-4834-a6ca-6f598ce3cdf7_6dbd2209-9d14-4c76-b92b-fcb00e835fe1",
  "createdBy": "admin@contoso.onmicrosoft.com",
  "createdDateTime": "2020-08-21T19:56:00.6320729Z",
  "modifiedBy": "admin@contoso.onmicrosoft.com",
  "modifiedDateTime": "2020-08-21T19:56:00.6320729Z"
}
```

O pacote de acesso agora tem uma função de recurso, que é a associação de grupo. A função é atribuída a qualquer usuário que tenha o pacote de acesso.

### <a name="create-an-access-package-policy"></a>Criar uma política de pacote de acesso

Agora que você criou o pacote de acesso e adicionou recursos e funções, pode decidir quem pode acessá-lo criando uma política de pacote de acesso. Neste tutorial, você habilita a **conta Solicitante1** que você criou para solicitar acesso aos recursos no pacote de acesso. Para essa tarefa, você precisa destes valores:
- **id** do pacote de acesso para o valor da **propriedade accessPackageId**
- **id** da conta **de usuário Solicitante1** para o valor da **propriedade de id** em **allowedRequestors**
 
O valor da propriedade **durationInDays** permite que a conta **Solicitante1** acesse os recursos no pacote de acesso por até 30 dias. Grave o valor da **propriedade de ID** que será retornada para uso posteriormente neste tutorial. 

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
Content-type: application/json

{
  "accessPackageId": "88203d16-0e31-41d4-87b2-dd402f1435e9",
  "displayName": "Specific users",
  "description": "Specific users can request assignment",
  "accessReviewSettings": null,
  "durationInDays": 30,
  "requestorSettings": {
    "scopeType": "SpecificDirectorySubjects",
    "acceptRequests": true,
    "allowedRequestors": [
       {
         "@odata.type": "#microsoft.graph.singleUser",
         "isBackup": false,
         "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
         "description": "Requestor1"
       }
    ]
  },
  "requestApprovalSettings": {
    "isApprovalRequired": false,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": false,
    "approvalMode": "NoApproval",
    "approvalStages": []
  }
}
```

#### <a name="response"></a>Resposta

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentPolicies/$entity",
  "id": "db440482-1210-4a60-9b55-3ac7a72f63ba",
  "accessPackageId": "88203d16-0e31-41d4-87b2-dd402f1435e9",
  "displayName": "Specific users",
  "description": "Specific users can request assignment",
  "canExtend": false,
  "durationInDays": 30,
  "expirationDateTime": null,
  "createdBy": "admin@contoso.onmicrosoft.com",
  "createdDateTime": "2020-06-29T19:47:44.7399675Z",
  "modifiedBy": "admin@contoso.onmicrosoft.com",
  "modifiedDateTime": "2020-06-29T19:47:44.7555489Z",
  "accessReviewSettings": null,
  "requestorSettings": {
    "scopeType": "SpecificDirectorySubjects",
    "acceptRequests": true,
    "allowedRequestors": [
      {
        "@odata.type": "#microsoft.graph.singleUser",
        "isBackup": false,
        "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
        "description": "Requestor1"
      }
    ]
  },
  "requestApprovalSettings": {
    "isApprovalRequired": false,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": false,
    "approvalMode": "NoApproval",
    "approvalStages": []
  }
}
```

## <a name="step-3-request-access"></a>Etapa 3: Solicitar acesso

Nesta etapa, a conta **de usuário Solicitante1** solicita acesso aos recursos no pacote de acesso.

Para solicitar acesso aos recursos no pacote de acesso, você precisa fornecer estes valores:
- **id** da conta **de usuário Solicitante1** que você criou para o valor da **propriedade targetId**
- **id** da diretiva de atribuição para o valor da **propriedade assignmentPolicyId**
- **id** do pacote de acesso para o valor da **propriedade accessPackageId**

Na resposta, você pode ver o status **de Aceito e** um estado de **Enviado.** Registrar o valor da **propriedade de ID** retornada para obter o status da solicitação mais tarde.

Se você ainda não fez isso, saia da conta de administrador que estava usando no Microsoft Graph Explorer. Entre na conta **de usuário Solicitante1** que você criou. Você será solicitado a alterar a senha se for a primeira vez que você estiver fazendo login.

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "UserAdd",
  "accessPackageAssignment":{
     "targetId":"007d1c7e-7fa8-4e33-b678-5e437acdcddc",
     "assignmentPolicyId":"db440482-1210-4a60-9b55-3ac7a72f63ba",
     "accessPackageId":"88203d16-0e31-41d4-87b2-dd402f1435e9"
  }
}
```

#### <a name="response"></a>Resposta

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",
    "createdDateTime": null,
    "completedDate": null,
    "id": "a6bb6942-3ae1-4259-9908-0133aaee9377",
    "requestType": "UserAdd",
    "requestState": "Submitted",
    "requestStatus": "Accepted",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": null
}
```

## <a name="step-4-validate-that-access-has-been-assigned"></a>Etapa 4: Validar se o acesso foi atribuído

Nesta etapa, confirme se a conta de usuário **Solicitante1** foi atribuída ao pacote de acesso e que agora ele é membro do grupo de recursos **marketing.**

Saia da conta solicitante1 e entre novamente na conta de administrador para ver o status da solicitação.

### <a name="get-the-status-of-the-request"></a>Obter o status da solicitação

Use o valor da **propriedade de ID** da solicitação para obter o status atual dela. Na resposta, você pode ver o status alterado para **Fulfilled** e o estado alterado para **Entregue.**

#### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/a6bb6942-3ae1-4259-9908-0133aaee9377
```

#### <a name="response"></a>Resposta

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",
  "createdDateTime": "2020-06-29T20:24:24.683Z",
  "completedDate": "2020-06-29T20:24:47.937Z",
  "id": "a6bb6942-3ae1-4259-9908-0133aaee9377",
  "requestType": "UserAdd",
  "requestState": "Delivered",
  "requestStatus": "FulfilledNotificationTriggered",
  "isValidationOnly": false,
  "expirationDateTime": null,
  "justification": null
}
```

### <a name="get-access-package-assignments"></a>Obter atribuições de pacote de acesso

Você também pode usar a **id** da política de pacote de acesso que você criou para ver se os recursos foram atribuídos à conta de usuário **Solicitante1.**

#### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=accessPackageAssignmentPolicy/Id eq 'db440482-1210-4a60-9b55-3ac7a72f63ba'
```

#### <a name="response"></a>Resposta

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignments",
  "value": [
    {
      "id": "a6bb6942-3ae1-4259-9908-0133aaee9377",
      "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
      "accessPackageId": "88203d16-0e31-41d4-87b2-dd402f1435e9",
      "assignmentPolicyId": "db440482-1210-4a60-9b55-3ac7a72f63ba",
      "targetId": "2bc42425-6dc5-4f2a-9ebb-7a7464481eb0",
      "assignmentStatus": "Delivered",
      "assignmentState": "Delivered",
      "isExtended": false,
      "expiredDateTime": null
    }
  ]
}
```

### <a name="get-the-members-of-the-group"></a>Obter os membros do grupo

Depois que a solicitação for concedida, você poderá usar a **id** registrada para o grupo de recursos **marketing** para ver se a conta de usuário **Solicitante1** foi adicionada a ela.

#### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/v1.0/groups/e93e24d1-2b65-4a6c-a1dd-654a12225487/members
```

#### <a name="response"></a>Resposta:

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "businessPhones": [],
      "city": null,
      "createdDateTime": "2020-06-23T18:43:24Z",
      "creationType": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "department": null,
      "displayName": "Requestor1",
      "employeeId": null,
      "faxNumber": null,
      "givenName": null,
      "imAddresses": [],
      "infoCatalogs": [],
      "isResourceAccount": null,
      "jobTitle": null,
      "legalAgeGroupClassification": null,
      "mail": null,
      "mailNickname": "Requestor1"
    }
  ]
}
```

## <a name="step-5-clean-up-resources"></a>Etapa 5: Limpar recursos

Nesta etapa, remova as alterações feitas e exclua o pacote de acesso da Campanha de **Marketing.**

### <a name="remove-an-access-package-assignment"></a>Remover uma atribuição de pacote de acesso

Você deve remover todas as atribuições do pacote de acesso antes de excluí-lo. Use a **id da** solicitação de atribuição que você gravou anteriormente para excluí-la.

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "AdminRemove",
  "accessPackageAssignment":{
     "id": "a6bb6942-3ae1-4259-9908-0133aaee9377"
  }
}
```

#### <a name="response"></a>Resposta

```http
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",
    "createdDateTime": null,
    "completedDate": null,
    "id": "78eaee8c-e6cf-48c9-8f99-aae44c35e379",
    "requestType": "AdminRemove",
    "requestState": "Submitted",
    "requestStatus": "Accepted",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": null
}
```

### <a name="delete-the-access-package-assignment-policy"></a>Excluir a política de atribuição do pacote de acesso

Use a **id da** diretiva de atribuição que você gravou anteriormente para excluí-la. Certifique-se de que todas as atribuições foram removidas primeiro.

#### <a name="request"></a>Solicitação

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/6c1f65ec-8c25-4a45-83c2-a1de2a6d0e9f
```

#### <a name="response"></a>Resposta

```http
No Content - 204
```

### <a name="delete-the-access-package"></a>Excluir o pacote de acesso

Use a **id do** pacote de acesso que você gravou anteriormente para excluí-lo.

#### <a name="request"></a>Solicitação

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/cf54c6ca-d717-49bc-babe-d140d035dfdd
```

#### <a name="response"></a>Resposta

```http
No Content - 204
```

### <a name="delete-the-user-account"></a>Excluir a conta de usuário

Exclua **a conta de usuário Solicitante1.**

#### <a name="request"></a>Solicitação

```http
DELETE https://graph.microsoft.com/v1.0/users/ce02eca8-752b-4ecf-ac29-aa9bccd87606
```

#### <a name="response"></a>Resposta

```http
No Content - 204
```

### <a name="delete-the-group"></a>Adicionar ou remover membros do grupo

Exclua o **grupo de recursos marketing.**

#### <a name="request"></a>Solicitação

```http
DELETE https://graph.microsoft.com/v1.0/groups/a468eaea-ed6c-4290-98d2-a96bb1cb4209
```

#### <a name="response"></a>Resposta

```http
No Content - 204
```

## <a name="see-also"></a>Confira também

Neste tutorial, você usou muitas APIs para realizar tarefas. Explore a referência de API para essas APIs para saber mais sobre o que as APIs podem fazer.


- [Trabalhar com a API de gerenciamento de direitos do Azure AD](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta)
- [accessPackageCatalog](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta)
- [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta)
- [accessPackage](/graph/api/resources/accesspackage?view=graph-rest-beta)
- [accessPackageResourceRoleScope](/graph/api/resources/accesspackageresourcerolescope?view=graph-rest-beta)
- [accessPackageAssignmentPolicy](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta)
- [accessPackageAssignmentRequest](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta)
- [group](/graph/api/resources/group?view=graph-rest-1.0)
- [user](/graph/api/resources/user?view=graph-rest-1.0)