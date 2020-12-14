---
title: 'Tutorial: identificar e corrigir riscos usando as APIs do Microsoft Graph'
description: Saiba como identificar e corrigir riscos usando as APIs do Microsoft Graph.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0bec8dc51c81b9d2d0349294c0f0d1f6bd4c1e98
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664163"
---
# <a name="tutorial-identify-and-remediate-risks-using-microsoft-graph-apis"></a>Tutorial: identificar e corrigir riscos usando as APIs do Microsoft Graph

O Azure AD Identity Protection fornece às organizações informações sobre riscos baseados em identidade e diferentes maneiras de investigar e corrigir automaticamente o risco. As APIs de proteção de identidade usadas neste tutorial podem ajudá-lo a identificar riscos e configurar um fluxo de trabalho para confirmar o comprometimento ou habilitar a correção. Para obter mais informações, consulte [o que é risco?](/azure/active-directory/identity-protection/concept-identity-protection-risks)

Neste tutorial, você aprenderá a gerar um usuário arriscado e a corrigir o status arriscado do usuário com uma política de acesso condicional que requer autenticação multifator (MFA). Uma seção opcional mostra como bloquear o usuário de entrar também usando uma política de acesso condicional e descartar o risco do usuário.

>**Observação:** Os objetos de resposta mostrados neste tutorial podem ser reduzidos para facilitar a leitura. 

## <a name="prerequisites"></a>Pré-requisitos

Para concluir com êxito este tutorial, verifique se você tem os pré-requisitos necessários:

- Você deve ter uma licença do Azure AD Premium P1 ou P2 para usar a API de detecção de risco.
- Este tutorial usa o navegador do Tor para entrar no portal do Azure anonimamente. Você pode usar qualquer navegador anônimo para realizar a tarefa. Para baixar o navegador do Tor, consulte [Download Tor browser](https://www.torproject.org/download/).
- Este tutorial pressupõe que você está usando o Microsoft Graph Explorer, mas você pode usar o postmaster ou criar seu próprio aplicativo cliente para chamar o Microsoft Graph. Para chamar as APIs do Microsoft Graph neste tutorial, você precisa usar uma conta com a função de administrador global e as permissões apropriadas. Conclua as seguintes etapas para definir permissões no Microsoft Graph Explorer:
    1. Iniciar [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).
    2. Selecione **entrar com a Microsoft** e entre usando uma conta de administrador global do Azure AD. Após entrar com êxito, você poderá ver os detalhes da conta de usuário no painel esquerdo.
    3. Selecione o ícone de configurações à direita dos detalhes da conta de usuário e selecione **permissões**.

        ![Definir permissões](./images/tutorial-riskdetection-api/set-permissions.png)
        
    4. Role a lista de permissões para estas permissões:
        - **IdentityRiskEvents (2)**, expanda e selecione `IdentityRiskEvent.Read.All`
        - **Identityriskuser (2)**, expanda e selecione `IdentityRiskyUser.ReadWrite.All`
        - **Política (13)**, expanda e, em seguida, selecione `Policy.Read.All` e `Policy.ReadWrite.ConditionalAccess`
        - **Usuário (8)**, expanda e selecione `User.ReadWrite.All`
        
        ![Pesquisar permissões](./images/tutorial-riskdetection-api/permissions-consent.png)
    
    5. Selecione **consentimento** e, em seguida, selecione **aceitar** para aceitar o consentimento das permissões. Você não precisa consentir em nome da sua organização para essas permissões.

        ![Aceitar permissões](./images/tutorial-riskdetection-api/accept-permissions.png)

## <a name="step-1-create-a-user-account"></a>Etapa 1: criar uma conta de usuário

Para este tutorial, você cria uma conta de usuário que é usada para testar as detecções de risco. No corpo da solicitação, mude `contoso.com` para o nome de domínio do seu locatário. Você pode encontrar informações sobre o locatário na página Visão geral do Azure Active Directory.

### <a name="request"></a>Solicitação

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled":true,
  "displayName":"MyTestUser1",
  "mailNickname":"MyTestUser1",
  "userPrincipalName":"MyTestUser1@contoso.com",
  "passwordProfile": {
    "forceChangePasswordNextSignIn":true,
    "password":"Contoso1234"
  }
}
```

### <a name="response"></a>Resposta

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
  "id": "4628e7df-dff3-407c-a08f-75f08c0806dc",
  "businessPhones": [],
  "displayName": "MyTestUser1",
  "givenName": null,
  "jobTitle": null,
  "mail": null,
  "mobilePhone": null,
  "officeLocation": null,
  "preferredLanguage": null,
  "surname": null,
  "userPrincipalName": "MyTestUser1@contoso.com"
}
```

## <a name="step-2-trigger-a-risk-detection"></a>Etapa 2: disparar uma detecção de risco

### <a name="trigger-a-risk-detection"></a>Acionar uma detecção de risco

Uma maneira de acionar uma detecção de risco em uma conta de usuário é fazer logon no portal do Azure anonimamente. Neste tutorial, o navegador do Tor é usado para entrar anonimamente. 

1. Abra o navegador e insira `portal.azure.com` o endereço do site.
2. Entre no portal usando as credenciais da conta do **MyTestUser1** que você criou anteriormente. Você será solicitado a alterar a senha existente.

### <a name="list-risk-detections"></a>Listar detecções de riscos

Quando você entrou no portal do Azure usando o navegador anônimo, um `anonymizedIPAddress` evento de risco foi detectado. Você pode usar o `$filter` parâmetro de consulta para obter apenas as detecções de risco associadas à conta de usuário **MyTestUser1** .

#### <a name="request"></a>Solicitação

``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections?$filter=userDisplayName eq 'MyTestUser1'
```

#### <a name="response"></a>Resposta

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#riskDetections",
  "value": [
    {
      "id": "d52a631815aaa527bf642b196715da5cf0f35b6879204ea5b5c99b21bd4c16f4",
      "requestId": "06f7fd18-b8f1-407d-86a3-f6cbe3a4be00",
      "correlationId": "2a38abff-5701-4073-a81e-fd3aac09cba3",
      "riskType": "anonymizedIPAddress",
      "riskEventType": "anonymizedIPAddress",
      "riskState": "atRisk",
      "riskLevel": "medium",
      "riskDetail": "none",
      "source": "IdentityProtection",
      "detectionTimingType": "realtime",
      "activity": "signin",
      "tokenIssuerType": "AzureAD",
      "ipAddress": "178.17.170.23",
      "activityDateTime": "2020-11-03T20:51:34.6245276Z",
      "detectedDateTime": "2020-11-03T20:51:34.6245276Z",
      "lastUpdatedDateTime": "2020-11-03T20:53:12.1984203Z",
      "userId": "4628e7df-dff3-407c-a08f-75f08c0806dc",
      "userDisplayName": "MyTestUser1",
      "userPrincipalName": "MyTestUser1@contoso.com",
      "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; rv:78.0) Gecko/20100101 Firefox/78.0\"}]",
      "location": {
        "city": "Chisinau",
        "state": "Chisinau",
        "countryOrRegion": "MD",
        "geoCoordinates": {
          "latitude": 47.0269,
          "longitude": 28.8416
        }
      }
    }
  ]
}
```

> **Observação:** Pode levar alguns minutos até que o evento seja retornado.

## <a name="step-3-create-a-conditional-access-policy"></a>Etapa 3: criar uma política de acesso condicional

Você pode aproveitar as políticas de acesso condicional em sua organização para permitir que os usuários façam a correção automática quando o risco for detectado. A AutoCorreção permite que os usuários se desbloqueiem para acessar seus recursos de forma segura após a conclusão do prompt da política. Nesta etapa, você criará uma política de acesso condicional que requer que o usuário entre usando a MFA se ocorrer uma detecção de alto risco.

### <a name="set-up-multi-factor-authentication"></a>Configurar a autenticação multifator

Ao configurar uma conta para a MFA, você pode escolher entre vários métodos para autenticar o usuário. Escolha o melhor método para a sua situação para concluir este tutorial. 

1. Entre no para [manter seu site seguro de conta](https://aka.ms/MFASetup) usando a conta **MyTestUser1** .
2. Conclua o procedimento de configuração da MFA usando o método apropriado para a sua situação, como ter uma mensagem de texto enviada ao seu telefone.

### <a name="create-the-conditional-access-policy"></a>Criar a política de acesso condicional

A política de acesso condicional fornece a capacidade de definir as condições da política para identificar os níveis de risco de entrada. Os níveis de risco podem ser `low` , `medium` , `high` , `none` . Na resposta retornada pela listar as detecções de risco para o **MyTestUser1**, podemos ver que o nível de risco é `medium` . Este exemplo mostra como exigir a MFA de **MyTestUser1** que foi identificada como um usuário arriscado.

#### <a name="request"></a>Solicitação 

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies 
Content-type: application/json
 
{ 
  "displayName": "Policy for risky sign-in", 
  "state": "enabled", 
  "conditions": { 
    "signInRiskLevels": [ 
      "high", 
      "medium" 
    ], 
    "applications": { 
      "includeApplications": ["All"]
    }, 
    "users": { 
      "includeUsers": [ 
        "4628e7df-dff3-407c-a08f-75f08c0806dc" 
      ] 
    } 
  }, 
  "grantControls": { 
    "operator": "OR", 
    "builtInControls": [ 
      "mfa" 
    ] 
  } 
} 
```

#### <a name="response"></a>Resposta 

```
{ 
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/conditionalAccess/policies/$entity", 
  "id": "9ad78153-b1f8-4714-adc1-1445727678a8", 
  "displayName": "Policy for risky sign-in", 
  "createdDateTime": "2020-11-03T20:56:38.6210843Z", 
  "modifiedDateTime": null, 
  "state": "enabled", 
  "sessionControls": null, 
  "conditions": { 
    "signInRiskLevels": [ 
      "high", 
      "medium" 
    ], 
    "clientAppTypes": [  
      "all"  
    ], 
    "platforms": null, 
    "locations": null, 
    "applications": { 
      "includeApplications": [ 
        "All" 
      ], 
      "excludeApplications": [], 
      "includeUserActions": [] 
    }, 
    "users": { 
      "includeUsers": [ 
        "4628e7df-dff3-407c-a08f-75f08c0806dc" 
      ], 
      "excludeUsers": [], 
      "includeGroups": [], 
      "excludeGroups": [], 
      "includeRoles": [], 
      "excludeRoles": [] 
    } 
  }, 
  "grantControls": { 
    "operator": "OR", 
    "builtInControls": [ 
      "mfa" 
    ], 
    "customAuthenticationFactors": [], 
    "termsOfUse": [] 
  } 
} 
```

Com essa política de acesso condicional in-loco, a conta **MyTestUser1**   agora é necessária para usar MFA ao entrar porque o nível de risco de entrada é médio ou alto. 

### <a name="sign-in-and-complete-multi-factor-authentication"></a>Entrar e concluir a autenticação multifator 

Ao entrar no navegador anônimo, um risco é detectado, mas é corrigido pela conclusão da MFA. 

1. Abra o navegador e insira  `portal.azure.com`   o endereço do site. 
2. Entre no portal usando as credenciais da conta **MyTestUser1**   e conclua o processo de MFA. 

### <a name="list-risk-detections"></a>Listar detecções de riscos

Porque a MFA foi concluída. Agora, quando você listar as detecções de risco, o **riscostate** mostrará o evento como `remediated` .

#### <a name="request"></a>Solicitação

``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections?$filter=userDisplayName eq 'MyTestUser1'
```

#### <a name="response"></a>Resposta

```http
{
  "id": "ba9d45f16d8f87f6ae974efda7336b2120962a398cb362dfd9e5bdc8e9d149d0",
  "requestId": "156c01fb-31cf-4a10-b9a9-beee93e6a400",
  "correlationId": "a8aaac45-fe22-46df-babf-10a8dba85d62",
  "riskType": "anonymizedIPAddress",
  "riskEventType": "anonymizedIPAddress",
  "riskState": "remediated",
  "riskLevel": "medium",
  "riskDetail": "userPassedMFADrivenByRiskBasedPolicy",
  "source": "IdentityProtection",
  "detectionTimingType": "realtime",
  "activity": "signin",
  "tokenIssuerType": "AzureAD",
  "ipAddress": "185.220.101.213",
  "activityDateTime": "2020-11-12T23:45:22.4092789Z",
  "detectedDateTime": "2020-11-12T23:45:22.4092789Z",
  "lastUpdatedDateTime": "2020-11-12T23:47:57.7831423Z",
  "userId": "4b608561-9258-44ba-8cdb-3286dcbf0e3b",
  "userDisplayName": "MyTestUser1",
  "userPrincipalName": "MyTestUser1@contoso.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; rv:78.0) Gecko/20100101 Firefox/78.0\"}]",
  "location": {
    "city": "Schoenwalde-Glien",
    "state": "Brandenburg",
    "countryOrRegion": "DE",
    "geoCoordinates": {
      "latitude": 52.61983,
      "longitude": 13.12743
    }
  }
}
```

## <a name="step-4-optional-block-the-user-from-signing-in"></a>Etapa 4 (opcional) bloquear o usuário de entrar

Em vez de fornecer a oportunidade para que o usuário seja automaticamente remediado, você pode impedir que o usuário entre. Nesta etapa, você cria uma nova política de acesso condicional que impede o usuário de entrar se ocorrer uma detecção de risco médio ou alto. A diferença nas políticas é que o **builtInControls** está definido como `block` .

### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies
Content-type: application/json

{
  "displayName": "Policy for risky sign-in block access",
  "state": "enabled",
  "conditions": {
    "signInRiskLevels": [
      "high",
      "medium"
    ],
    "applications": {
      "includeApplications": ["All"]
    },
    "users": {
      "includeUsers": [
        "4628e7df-dff3-407c-a08f-75f08c0806dc"
      ]
    }
  },
  "grantControls": {
    "operator": "OR",
    "builtInControls": [
      "block"
    ]
  }
}
```

### <a name="response"></a>Resposta

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/conditionalAccess/policies/$entity",
  "id": "9ad78153-b1f8-4714-adc1-1445727678a8",
  "displayName": "Policy for risky sign-in block access",
  "createdDateTime": "2020-11-03T20:56:38.6210843Z",
  "modifiedDateTime": null,
  "state": "enabled",
  "sessionControls": null,
  "conditions": {
    "signInRiskLevels": [
      "high",
      "medium"
    ],
    "clientAppTypes": [ 
      "all" 
    ],
    "platforms": null,
    "locations": null,
    "applications": {
      "includeApplications": [
        "All"
      ],
      "excludeApplications": [],
      "includeUserActions": []
    },
    "users": {
      "includeUsers": [
        "4628e7df-dff3-407c-a08f-75f08c0806dc"
      ],
      "excludeUsers": [],
      "includeGroups": [],
      "excludeGroups": [],
      "includeRoles": [],
      "excludeRoles": []
    }
  },
  "grantControls": {
    "operator": "OR",
    "builtInControls": [
      "block"
    ],
    "customAuthenticationFactors": [],
    "termsOfUse": []
  }
}
```

Com essa política de acesso condicional in-loco, a conta do **MyTestUser1** agora está impedida de entrar porque o nível de risco de entrada é `medium` ou `high` .

![Entrada bloqueada](./images/tutorial-riskdetection-api/conditionalaccess-policy.png)

## <a name="step-5-dismiss-risky-users"></a>Etapa 5: ignorar usuários arriscados

Se acreditar que o usuário não está em risco e você não deseja impor uma política de acesso condicional, você pode descartar manualmente o usuário arriscado.

### <a name="dismiss-the-risky-user"></a>Ignorar o usuário arriscado

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss
Content-Type: application/json

{
  "userIds": [
    "4628e7df-dff3-407c-a08f-75f08c0806dc"
  ]
}
```

#### <a name="response"></a>Resposta

```http
HTTP/1.1 204 No Content
```        

### <a name="list-risky-users"></a>Listar usuários arriscados

Após descartar o usuário de risco, você poderá ver na resposta ao listar os usuários arriscados que a conta de usuário do **MyTestUser1** agora tem um nível de risco `none` e um risco de `dismissed` .

#### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers?$filter=userDisplayName eq 'MyTestUser1'
```

#### <a name="response"></a>Resposta

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#riskyUsers",
  "value": [
    {
      "id": "4628e7df-dff3-407c-a08f-75f08c0806dc",
      "isDeleted": false,
      "isProcessing": false,
      "riskLevel": "none",
      "riskState": "dismissed",
      "riskDetail": "adminDismissedAllRiskForUser",
      "riskLastUpdatedDateTime": "2020-11-03T21:48:53.4298425Z",
      "userDisplayName": "MyTestUser1",
      "userPrincipalName": "MyTestUser1@contoso.com"
    }
  ]
}
```

## <a name="step-6-clean-up-resources"></a>Etapa 6: limpar recursos

Nesta etapa, remova os recursos que você criou.

### <a name="delete-the-user-account"></a>Excluir a conta de usuário

Exclua a conta de usuário do **MyTestUser1** .

#### <a name="request"></a>Solicitação

```http
DELETE https://graph.microsoft.com/v1.0/users/4628e7df-dff3-407c-a08f-75f08c0806dc
```

#### <a name="response"></a>Resposta

```http
No Content - 204
```

### <a name="delete-the-conditional-access-policy"></a>Excluir a política de acesso condicional

Exclua a política de acesso condicional que você criou.

#### <a name="request"></a>Solicitação

```http
DELETE https://graph.microsoft.com/v1.0/groups/9ad78153-b1f8-4714-adc1-1445727678a8
```

#### <a name="response"></a>Resposta

```http
No Content - 204
```

## <a name="see-also"></a>Confira também

Neste tutorial, você usou muitas APIs para realizar tarefas. Explore a referência de API para essas APIs para saber mais sobre o que as APIs podem fazer.

- [O que é proteção de identidade?](/azure/active-directory/identity-protection/overview-identity-protection)
- [O que é Acesso Condicional?](/azure/active-directory/conditional-access/overview)
- [Como funciona: autenticação multifator do Azure](/azure/active-directory/authentication/concept-mfa-howitworks)
- [conditionalAccessPolicy](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-1.0)
- [riskDetection](/graph/api/resources/riskdetection?view=graph-rest-1.0)
- [riskyUser](/graph/api/resources/riskyuser?view=graph-rest-1.0)
- [user](/graph/api/resources/user?view=graph-rest-1.0)