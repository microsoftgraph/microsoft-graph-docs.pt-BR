---
title: 'Tutorial: Usar a API Privileged Identity Management (PIM) para atribuir Azure AD funções'
description: Saiba como usar a API Privileged Identity Management (PIM) no Microsoft Graph para atribuir funções Azure AD privilegiadas.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: 78e523a12d59ac7b25482da26f3fb594e9517657
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247186"
---
# <a name="tutorial-use-the-privileged-identity-management-pim-api-to-assign-azure-ad-roles"></a>Tutorial: Usar a API Privileged Identity Management (PIM) para atribuir Azure AD funções

A API Graph PIM da Microsoft permite que as organizações gerenciem o acesso privilegiado a recursos Azure Active Directory (Azure AD). Ele também ajuda a gerenciar os riscos de acesso privilegiado limitando quando o acesso está ativo, gerenciando o escopo de acesso e fornecendo um log auditável de acesso privilegiado.

Neste tutorial, uma empresa fictícia chamada Contoso Limited deseja que sua Assistência Técnica de TI gerencie o ciclo de vida do acesso dos funcionários. A empresa identificou a função Azure AD Administrador de Usuários como a função privilegiada apropriada exigida pela Assistência Técnica de TI e usará a API do PIM para atribuir a função.

Você criará um grupo de segurança atribuível a funções para a Assistência Técnica de TI e, usando a API do PIM, atribuirá a elegibilidade do grupo de segurança à função de Administrador do Usuário. Ao atribuir a função qualificada a um grupo de segurança, a Contoso tem uma maneira mais eficiente de gerenciar o acesso de administrador a recursos como funções Azure AD segurança. Por exemplo:

+ A remoção ou a adição de mais membros do grupo também remove os administradores.
+ Adicionar mais funções aos membros do grupo em vez de atribuir funções a usuários individuais.

Atribuir qualificação em vez de um privilégio de Administrador de Usuário persistentemente ativo permite que a empresa imponha o acesso **Just-In-Time**, que concede permissões temporárias para executar as tarefas privilegiadas. Depois de definir a qualificação de função, o membro do grupo qualificado ativa sua atribuição por um período temporário. Todos os registros de ativações de função serão auditáveis pela empresa.

>[!NOTE]
>Os objetos de resposta mostrados neste tutorial podem ser reduzidos para legibilidade.

## <a name="prerequisites"></a>Pré-requisitos

Para concluir este tutorial, você precisa dos seguintes recursos e privilégios:

+ Um locatário Azure AD trabalho com uma licença Azure AD Premium P2 ou EMS E5 habilitada.
+ Entre no [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) como um usuário em uma função de Administrador Global.
  + [Opcional] Inicie uma nova sessão anônima ou inprivate do navegador ou inicie uma sessão em um navegador anônimo. Você entrará mais adiante neste tutorial.
+ As seguintes permissões delegadas: `User.ReadWrite.All`, `Group.ReadWrite.All`, `Directory.Read.All`, `RoleEligibilitySchedule.ReadWrite.Directory`e `RoleAssignmentSchedule.ReadWrite.Directory`, e .`RoleManagement.ReadWrite.Directory`
+ Authenticator aplicativo instalado em seu telefone para registrar um usuário para autenticação multifator (MFA).

Para consentir com as permissões necessárias no Graph Explorer:
1. Selecione o ícone de reticências horizontais à direita dos detalhes da conta de usuário e escolha **Selecionar permissões**.
  
      :::image type="content" source="/graph/images/GE-Permissions/selectpermissions.png" alt-text="Selecione permissões Graph Microsoft." border="true":::

2. Percorra a lista de permissões para estas permissões:
    + Agrupar (2), expandir e selecionar **Group.ReadWrite.All**.
    + Diretório (4), expanda e selecione **Directory.Read.All**.
    + RoleAssignmentSchedule (2), expanda e selecione **RoleAssignmentSchedule.ReadWrite.Directory**.
    + RoleEligibilitySchedule (2), expanda e selecione **RoleEligibilitySchedule.ReadWrite.Directory**.
    + RoleManagement (3), expanda e selecione **RoleManagement.ReadWrite.Directory**.
    + Usuário (8), expanda e selecione **User.ReadWrite.All**.
   
   Selecione **Consentimento** e, em seguida, selecione **Aceitar** para aceitar o consentimento das permissões. Para permissões `RoleEligibilitySchedule.ReadWrite.Directory` e `RoleAssignmentSchedule.ReadWrite.All` permissões, consenta em nome de sua organização.

      :::image type="content" source="/graph/images/GE-Permissions/User.ReadWrite.All-consent.png" alt-text="Consentir com permissões Graph Microsoft." border="true":::

## <a name="step-1-create-a-test-user"></a>Etapa 1: Criar um usuário de teste

Crie um usuário que deve redefinir sua senha na primeira entrada. Nesta etapa, registre o valor da **ID** do novo usuário para uso na próxima etapa. Depois de criar o usuário, visite o portal do Azure e habilite a MFA (autenticação multifator) para o usuário. Para obter mais informações sobre como habilitar a MFA, consulte a [seção](#see-also) Consulte também.


### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-createUser"
}-->
```http
POST https://graph.microsoft.com/v1.0/users
Content-Type: application/json

{
    "accountEnabled": true,
    "displayName": "Aline Dupuy",
    "mailNickname": "AlineD",
    "userPrincipalName": "AlineD@Contoso.com",
    "passwordProfile": {
        "forceChangePasswordNextSignIn": true,
        "password": "xWwvJ]6NMw+bWH-d"
    }
}
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/29a4f813-9274-4e1b-858d-0afa98ae66d4/directoryObjects/7146daa8-1b4b-4a66-b2f7-cf593d03c8d2/Microsoft.DirectoryServices.User",
    "id": "7146daa8-1b4b-4a66-b2f7-cf593d03c8d2",
    "displayName": "Aline Dupuy",
    "userPrincipalName": "AlineD@Contoso.com"
}
```

## <a name="step-2-create-a-security-group-that-can-be-assigned-an-azure-ad-role"></a>Etapa 2: Criar um grupo de segurança que pode ser atribuído a uma Azure AD função

Crie um grupo que seja atribuível a uma Azure AD função. Atribua-se como o proprietário do grupo e você e a Aline (o usuário criado na Etapa 1) como membros.

### <a name="request-create-a-role-assignable-group"></a>Solicitação: Criar um grupo atribuível à função

Substitua `1ed8ac56-4827-4733-8f80-86adc2e67db5` pela ID e `7146daa8-1b4b-4a66-b2f7-cf593d03c8d2` pelo valor da ID de Aline.

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-createSecurityGroup"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json

{
    "description": "IT Helpdesk to support Contoso employees",
    "displayName": "IT Helpdesk (User)",
    "mailEnabled": false,
    "mailNickname": "userHelpdesk",
    "securityEnabled": true,
    "isAssignableToRole": true,
    "owners@odata.bind": [
        "https://graph.microsoft.com/v1.0/users/1ed8ac56-4827-4733-8f80-86adc2e67db5"
    ],
    "members@odata.bind": [
        "https://graph.microsoft.com/v1.0/users/1ed8ac56-4827-4733-8f80-86adc2e67db5",
        "https://graph.microsoft.com/v1.0/users/7146daa8-1b4b-4a66-b2f7-cf593d03c8d2"
    ]
}
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/29a4f813-9274-4e1b-858d-0afa98ae66d4/directoryObjects/e77cbb23-0ff2-4e18-819c-690f58269752/Microsoft.DirectoryServices.Group",
    "id": "e77cbb23-0ff2-4e18-819c-690f58269752",
    "description": "IT Helpdesk to support Contoso employees",
    "displayName": "IT Helpdesk (User)",
    "groupTypes": [],
    "isAssignableToRole": true,
    "mailEnabled": false,
    "mailNickname": "userHelpdesk",
    "securityEnabled": true,
    "securityIdentifier": "S-1-12-1-3883711267-1310199794-258579585-1385637464",
    "visibility": "Private",
    "onPremisesProvisioningErrors": []
}
```

## <a name="step-3-create-a-unifiedroleeligibilityschedulerequest"></a>Etapa 3: Criar um unifiedRoleEligibilityScheduleRequest

Agora que você tem um grupo de segurança, atribua-o como qualificado para a função de Administrador do Usuário. Nesta etapa:

+ Crie um objeto unifiedRoleEligibilityScheduleRequest que identifique a Assistência Técnica **de TI do grupo (Usuário)** como qualificada para a função de Administrador de Usuários por um ano. Azure AD estende essa atribuição qualificada aos membros do grupo, ou seja, você e Aline.
+ Definir o escopo da atribuição qualificada para todo o locatário. Isso permite que o administrador do usuário use seu privilégio em relação a todos os usuários em seu locatário, exceto usuários com privilégios mais altos, como o Administrador Global.

### <a name="request"></a>Solicitação

Substitua `e77cbb23-0ff2-4e18-819c-690f58269752` pelo valor da **ID do** grupo de segurança **da Assistência Técnica** de TI (Usuário). Essa **principalId** identifica o destinatário da qualificação para a função de Administrador do Usuário. O roleDefinitionId `fe930be7-5e62-47db-91af-98c3a49a38b1` é o identificador de modelo global para a função de Administrador de Usuários no Azure AD.

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-unifiedRoleEligibilityScheduleRequest_create"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/roleManagement/directory/roleEligibilityScheduleRequests
Content-type: application/json

{
    "action": "AdminAssign",
    "justification": "Assign User Admin eligibility to IT Helpdesk (User) group",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "directoryScopeId": "/",
    "principalId": "e77cbb23-0ff2-4e18-819c-690f58269752",
    "scheduleInfo": {
        "startDateTime": "2021-07-01T00:00:00Z",
        "expiration": {
            "endDateTime": "2022-06-30T00:00:00Z",
            "type": "AfterDateTime"
        }
    }
}
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequests"
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
    "id": "64a8bd54-4591-4f6a-9c77-3e9cb1fdd29b",
    "status": "Provisioned",
    "createdDateTime": "2021-09-03T20:45:28.3848182Z",
    "completedDateTime": "2021-09-03T20:45:39.1194292Z",
    "action": "AdminAssign",
    "principalId": "e77cbb23-0ff2-4e18-819c-690f58269752",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "directoryScopeId": "/",
    "isValidationOnly": false,
    "targetScheduleId": "64a8bd54-4591-4f6a-9c77-3e9cb1fdd29b",
    "justification": "Assign User Admin eligibility to IT Helpdesk (User) group",
    "createdBy": {
        "user": {
            "id": "1ed8ac56-4827-4733-8f80-86adc2e67db5"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2021-09-03T20:45:39.1194292Z",
        "expiration": {
            "type": "afterDateTime",
            "endDateTime": "2022-06-30T00:00:00Z"
        }
    },
    "ticketInfo": {}
}
```

## <a name="step-4-confirm-the-users-current-role-assignments"></a>Etapa 4: Confirmar as atribuições de função atuais do usuário

Embora os membros do grupo agora estejam qualificados para a função de Administrador do Usuário, eles ainda não conseguem usar a função. Isso ocorre porque eles ainda não ativaram sua qualificação. Você pode confirmar verificando as atribuições de função atuais do usuário.


### <a name="request"></a>Solicitação

Na solicitação a seguir, substitua `7146daa8-1b4b-4a66-b2f7-cf593d03c8d2` pelo valor da **ID de Aline**.

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-roleAssignments_list"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignments?$filter=principalId eq '7146daa8-1b4b-4a66-b2f7-cf593d03c8d2'
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignments"
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleAssignments",
    "value": []
}
```

O objeto de resposta vazio mostra que Aline não tem funções Azure AD existentes na Contoso. O Aline agora ativará sua função de Administrador de Usuário qualificada por um tempo limitado.

## <a name="step-5-user-self-activates-their-eligible-assignment"></a>Etapa 5: o usuário ativa automaticamente sua atribuição qualificada

Um tíquete de incidente CONTOSO: Segurança-012345 foi gerado no sistema de gerenciamento de incidentes da Contoso e a empresa exige que todos os tokens de atualização do funcionário sejam invalidados. Como membro da Assistência Técnica de TI, a Aline é responsável por cumprir essa tarefa.

Primeiro, inicie o Authenticator em seu telefone e abra a conta de Aline Dupuy.

Entre no Graph Explorer como Aline. Você pode usar uma sessão anônima ou um navegador anônimo para esta etapa. Ao fazer isso, você não interromperá sua sessão atual como usuário na função de Administrador Global. Como alternativa, você pode interromper a sessão atual saindo do Graph Explorer e entrando novamente como Aline.

Conectado como Aline, primeiro você alterará sua senha porque ela foi especificada durante a criação da conta. Em seguida, como o administrador configurou sua conta para MFA, você será solicitado a configurar sua conta no aplicativo Authenticator e ser desafiado para entrar na MFA. Isso ocorre porque o PIM requer essa MFA para todas as atribuições de função ativas.

Depois de entrar, ative sua função de Administrador de Usuário por cinco horas.

### <a name="request"></a>Solicitação

Para ativar uma função, chame o ponto `roleAssignmentScheduleRequests` de extremidade. Nessa solicitação, a `UserActivate` ação permite ativar sua atribuição qualificada, nesse caso, por cinco horas.

+ Para **principalId**, forneça o valor da sua **ID** (de Aline).
+ A **roleDefinitionId** é a **ID** da função para a qual você está qualificado, nesse caso, a função de Administrador do Usuário.
+ Insira os detalhes do sistema de tíquetes que fornece uma justificativa auditável para ativar a solicitação.

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-roleAssignmentScheduleRequests_selfActivate"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleRequests
Content-type: application/json

{
    "action": "SelfActivate",
    "principalId": "7146daa8-1b4b-4a66-b2f7-cf593d03c8d2",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "directoryScopeId": "/",
    "justification": "Need to invalidate all app refresh tokens for Contoso users.",
    "scheduleInfo": {
        "startDateTime": "2021-09-04T15:13:00.000Z",
        "expiration": {
            "type": "AfterDuration",
            "duration": "PT5H"
        }
    },
    "ticketInfo": {
        "ticketNumber": "CONTOSO:Security-012345",
        "ticketSystem": "Contoso ICM"
    }
}
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.roleEligibilityScheduleRequests"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleAssignmentScheduleRequests/$entity",
    "id": "295edd40-4646-40ca-89b8-ab0b46b6f60e",
    "status": "Granted",
    "createdDateTime": "2021-09-03T21:10:49.6670479Z",
    "completedDateTime": "2021-09-04T15:13:00Z",
    "action": "SelfActivate",
    "principalId": "7146daa8-1b4b-4a66-b2f7-cf593d03c8d2",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "directoryScopeId": "/",
    "isValidationOnly": false,
    "targetScheduleId": "295edd40-4646-40ca-89b8-ab0b46b6f60e",
    "justification": "Need to invalidate all app refresh tokens for Contoso users.",
    "createdBy": {
        "user": {
            "id": "7146daa8-1b4b-4a66-b2f7-cf593d03c8d2"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2021-09-04T15:13:00Z",
        "expiration": {
            "type": "afterDuration",
            "endDateTime": null,
            "duration": "PT5H"
        }
    },
    "ticketInfo": {
        "ticketNumber": "CONTOSO:Security-012345",
        "ticketSystem": "Contoso ICM"
    }
}
```

Você pode confirmar sua atribuição executando `GET https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleRequests/filterByCurrentUser(on='principal')`. O objeto de resposta retorna sua atribuição de função recém-ativada com seu status definido como `Granted`. Com seu novo privilégio, execute todas as ações permitidas dentro de cinco horas para que sua atribuição esteja ativa. Isso inclui a invalidação dos tokens de atualização de todos os funcionários. Após cinco horas, a atribuição ativa expira, mas por meio de sua associação ao grupo de Suporte de **TI (** Usuários), você ainda permanece qualificado para a função de Administrador de Usuários.

De volta à sessão de administrador global, você recebeu notificações da atribuição qualificada e da ativação da função. Isso permite que o administrador global esteja ciente de todas as elevações aos privilégios de administrador em toda a sua organização.

## <a name="step-6-clean-up-resources"></a>Etapa 6: Limpar recursos

Entre como Administrador Global e exclua os seguintes recursos que você criou para este tutorial: a solicitação de qualificação de função, o grupo de Suporte de TI (Usuários) e o usuário de teste (Aline Dupuy).

### <a name="revoke-the-role-eligibility-request"></a>Revogar a solicitação de qualificação de função

#### <a name="request"></a>Solicitação

Substitua `e77cbb23-0ff2-4e18-819c-690f58269752` pela **ID do** grupo de Suporte de TI (Usuários).

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-roleEligibilityScheduleRequests_revoke"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/roleManagement/directory/roleEligibilityScheduleRequests
Content-type: application/json

{
    "action": "AdminRemove",
    "principalId": "e77cbb23-0ff2-4e18-819c-690f58269752",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "directoryScopeId": "/"
}

```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.roleEligibilityScheduleRequests"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
    "id": "dcd11a1c-300f-4d17-8c7a-523830400ec8",
    "status": "Revoked",
    "action": "AdminRemove",
    "principalId": "e77cbb23-0ff2-4e18-819c-690f58269752",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "directoryScopeId": "/"
}
```

### <a name="delete-the-it-support-users-group"></a>Excluir o grupo de Suporte de TI (Usuários)

#### <a name="request"></a>Solicitação

Substitua `e77cbb23-0ff2-4e18-819c-690f58269752` pela **ID do** grupo de Suporte de TI (Usuários).

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-group_delete"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/v1.0/groups/e77cbb23-0ff2-4e18-819c-690f58269752
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="delete-the-test-user"></a>Excluir o usuário de teste

#### <a name="request"></a>Solicitação

Substitua `7146daa8-1b4b-4a66-b2f7-cf593d03c8d2` pelo valor da **ID** de Aline.

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-user_delete"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/v1.0/users/7146daa8-1b4b-4a66-b2f7-cf593d03c8d2
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>Confira também

+ [Visão geral do gerenciamento de funções por meio do PIM](/graph/api/resources/privilegedidentitymanagementv3-overview)
+ [Azure AD funções internas](/azure/active-directory/roles/permissions-reference#all-roles)
+ [Habilitar a autenticação Azure AD multifator por usuário para proteger eventos de entrada](/azure/active-directory/authentication/howto-mfa-userstates)
+ [Tipo de recurso unifiedRoleEligibilityScheduleRequest](/graph/api/resources/unifiedroleeligibilityschedulerequest)