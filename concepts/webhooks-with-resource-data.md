---
title: Configurar notificações de alteração que incluam dados de recursos (visualização)
description: O Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. As notificações podem incluir propriedades do recurso.
author: baywet
ms.prod: non-product-specific
localization_priority: Priority
ms.openlocfilehash: 8f582ed08e97b3460259de23b564ec2bb9157750
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2020
ms.locfileid: "43805931"
---
# <a name="set-up-change-notifications-that-include-resource-data-preview"></a>Configurar notificações de alteração que incluam dados de recursos (visualização)

O Microsoft Graph permite que os aplicativos inscrevam-se para alterar as notificações de recursos através do [webhooks](webhooks.md). Agora você pode configurar assinaturas para incluir os dados de recursos alterados (como o conteúdo de uma mensagem de bate-papo do Microsoft Teams) em notificações. Em seguida, seu aplicativo pode usar a lógica de negócios sem ter que fazer uma chamada à API separada para buscar o recurso alterado. Como resultado, o aplicativo funciona melhor ao realizar menos chamadas da API, o que é benéfico em cenários de larga escala.

Incluir dados de recursos como parte de notificações exige que você implemente a seguinte lógica adicional para atender aos requisitos de acesso e segurança de dados: 

- [Lidar com](#subscription-life-cycle-notifications) as notificações do _ciclo de vida_ de assinatura especial para manter um fluxo ininterrupto de dados. O Microsoft Graph envia notificações do ciclo de vida de vez em quando para exigir que um aplicativo seja autorizado novamente, para garantir que os problemas de acesso não tenham sido cortados inesperadamente para incluir dados de recursos em notificações.
- [Valide](#validating-the-authenticity-of-notifications) a autenticidade das notificações como tendo sido originadas no Microsoft Graph.
- [Forneça](#decrypting-resource-data-from-change-notifications) uma chave de criptografia pública e use uma chave privada para descriptografar os dados de recursos recebidos através de notificações.

## <a name="resource-data-in-notification-payload"></a>Dados de recursos na carga de notificação 

Geralmente, esse tipo de notificação de alteração inclui os seguintes dados de recursos na carga:

- ID e tipo de instância de recurso alterado, retornados na propriedade **resourceData**.
- Todos os valores de propriedade da instância de recurso, criptografados conforme especificado na assinatura, retornados na propriedade **encryptedContent**.
- Or, dependendo do recurso, propriedades específicas retornadas na propriedade **resourceData**. Para obter somente propriedades específicas, especifique-as como parte da URL do **recurso** na assinatura, usando um parâmetro `$select`.  


## <a name="supported-resources"></a>Recursos com suporte

Atualmente, o recurso [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) (visualização) do Microsoft Teams oferece suporte a notificações de alteração que incluem dados de recursos. Especificamente, você pode configurar uma assinatura que se aplique a uma das seguintes opções:

- Mensagens novas ou alteradas em um canal específico do Teams: `/teams/{id}/channels/{id}/messages`
- Mensagens novas ou alteradas em um bate-papo específico do Teams: `/chats/{id}/messages`

O recurso **chatMessage** permite incluir todas as propriedades de uma instância alterada em uma notificação. Não há suporte para retornar apenas propriedades seletivas da instância. 

Este artigo mostra um exemplo de assinatura de alteração de notificações de mensagens em um canal do Teams, com cada notificação incluindo os dados de recursos totais da instância alterada **chatMessage**.

## <a name="creating-a-subscription"></a>Criar uma assinatura

Para que os dados de recursos estejam incluídos nas notificações de alteração, você **deve** especificar as seguintes propriedades, além das que geralmente são especificadas ao [criar uma assinatura](webhooks.md#creating-a-subscription):

- **includeResourceData** que deve ser definido como `true` para solicitar explicitamente os dados de recursos.
- **lifecycleNotificationUrl** é um ponto de extremidade onde as [notificações do ciclo de vida](#subscription-life-cycle-notifications) são fornecidas. Pode ser igual ou diferente de **notificationUrl**.
- **encryptionCertificate** que contém apenas a chave público que o Microsoft Graph usa para criptografar os dados de recursos. Mantenha a chave privada correspondente para [descriptografar o conteúdo](#decrypting-resource-data-from-change-notifications).
- **encryptionCertificateId** é o seu próprio identificador para o certificado. Use essa ID para corresponder a cada notificação, qual certificado usar para descriptografia.

Lembre-se do seguinte:

- Use o mesmo nome de host para os pontos de extremidade de notificação (**notificationUrl** e **lifecycleNotificationUrl**).
- Valide os dois pontos de extremidade de notificação conforme descrito [aqui](webhooks.md#notification-endpoint-validation). Se você quiser usar a mesma URL para os dois pontos de extremidade, você receberá e responderá a duas solicitações de validação.
- Não é possível atualizar (`PATCH`) uma assinatura existente para adicionar a propriedade **lifecycleNotificationUrl**. Você deve remover a assinatura existente e criar uma nova assinatura para incluir a propriedade **lifecycleNotificationUrl**.

### <a name="subscription-request-example"></a>Exemplo de solicitação de assinatura

O exemplo a seguir assina dois tipos de notificações: 

- Alterações de recursos - canais de mensagens sendo criados ou atualizados no Microsoft Teams
- Eventos do ciclo de vida da assinatura que podem afetar o fluxo das notificações de alteração. Veja mais detalhes sobre as notificações do ciclo de vida na [próxima seção](#subscription-life-cycle-notifications).

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="subscription-response"></a>Resposta de assinatura
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificateId": "{custom ID}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secret client state}"
}
```

## <a name="subscription-life-cycle-notifications"></a>Notificações do ciclo de vida da assinatura

Determinados eventos podem interferir no fluxo de notificação normal de uma assinatura existente. As _notificações do ciclo de vida_ da assinatura informam as ações necessárias para manter um fluxo ininterrupto. Ao contrário de uma notificação de alteração de recurso que informa uma alteração a uma instância de recurso, uma notificação do ciclo de vida trata-se da própria assinatura e seu estado atual no ciclo de vida. 

As notificações do ciclo de vida são fornecidas a **lifecycleNotificationUrl**. 

Nesta seção:

- [Notificação do ciclo de vida que desafia a autorização de assinatura](#life-cycle-notification-that-challenges-subscription-authorization)
- [Fluxo de desafio de autorização](#authorization-challenge-flow)
- [Exemplo de desafio de autorização](#example-authorization-challenge)
- [Respondendo a um desafio de autorização](#responding-to-an-authorization-challenge)
- [Dicas](#tips)
- [Proteja o seu código para lidar com outros tipos de notificações do ciclo de vida](#future-proof-your-code-to-handle-other-types-of-life-cycle-notifications)

### <a name="life-cycle-notification-that-challenges-subscription-authorization"></a>Notificação do ciclo de vida que desafia a autorização de assinatura 

Um tipo de notificações do ciclo de vida desafia o estado autorizado de uma assinatura ativa. Quando a propriedade **lifecycleEvent** em uma notificação indica `reauthorizationRequired`, você deve autorizar novamente a assinatura para manter o fluxo de dados.

Quando você cria uma assinatura de vida longa (por exemplo, uma que dura três dias), as notificações de dados de recursos fluem para o local indicado em **notificationUrl**. Entretanto, a qualquer momento, o Microsoft Graph pode exigir que você autorize novamente a assinatura para provar que ainda tem acesso aos dados de recursos, caso as condições de acesso tenham sido alteradas desde a criação da assinatura. A seguir estão exemplos de alterações que afetam o acesso aos dados:

- Um administrador de locatários pode revogar as permissões do seu aplicativo para ler um recurso.
- Em um cenário interativo, o usuário que fornece o token de autenticação ao seu aplicativo pode estar sujeito a políticas dinâmicas com base em vários fatores, como o local, o estado do dispositivo ou a avaliação de risco. Por exemplo, se o usuário alterar o seu local físico, pode ser que ele não tenha mais permissão para acessar os dados e seu aplicativo não conseguirá autorizar novamente a assinatura. Para saber mais sobre políticas dinâmicas que controlam o acesso, confira [políticas de acesso condicional do Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/overview). 

### <a name="authorization-challenge-flow"></a>Fluxo de desafio de autorização

O fluxo de um desafio de autorização para uma assinatura ativa e não expirada tem a seguinte aparência:

1. O Microsoft Graph exige que uma assinatura seja autorizada novamente.
    
    Os motivos para isso podem variar de recurso para recurso e podem mudar com o tempo. Independentemente da causa do evento de reautorização, você precisará respondê-lo.

2. O Microsoft Graph envia uma notificação de desafio de autorização para **lifecycleNotificationUrl**

    Observe que o fluxo de notificações de recursos pode continuar por algum tempo, dando a você mais tempo para responder. Entretanto, eventualmente a entrega da notificação de recursos será pausada, até que você execute a ação necessária.

3. Responda a essa notificação de duas maneiras:
    1. Autorize a assinatura novamente. Isso não estende a data de vencimento da assinatura.
    2. Renove a assinatura. Isso reautoriza e estenda a data de vencimento.

    Observação: as duas ações exigem a apresentação de um token de autenticação válido, semelhante a [criar uma nova assinatura](webhooks.md#creating-a-subscription) ou [renova uma assinatura antes da sua expiração](webhooks.md#renewing-a-subscription).

4. Se você conseguir autorizar novamente ou renovar a assinatura, as notificações de recursos continuarão. Caso contrário, as notificações de recursos permanecem em pausa.
    
### <a name="example-authorization-challenge"></a>Exemplo de desafio de autorização

Veja um exemplo de notificação de ciclo de vida que solicita a reautorização de uma assinatura. 

Observe o seguinte:

- O campo `"lifecycleEvent": "reauthorizationRequired"` identifica essa notificação como um desafio de autorização.
- A notificação não contém informações sobre um recurso específico, porque ela não está relacionada a uma alteração de recurso, mas a alteração de estado da assinatura.
- Assim como as notificações de recursos, as notificações do ciclo de vida podem estar em lote juntas (na coleção **valor**), cada uma com valores possivelmente diferentes **lifecycleEvent**. Processe cada notificação no lote de acordo.

```json
{
  "value": [
    {
      "lifecycleEvent": "reauthorizationRequired",
      "subscriptionId": "e3898f08-5cd0-4a6a-80fc-6addbfb73b7b",
      "subscriptionExpirationDateTime": "2019-09-18T00:52:45.9696658+00:00",
      "clientState": "{secret client state}",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95"
    }
  ]
}
```

### <a name="responding-to-an-authorization-challenge"></a>Respondendo a um desafio de autorização

Execute as etapas a seguir para processar uma notificação do ciclo de vida de desafio de autorização. As duas primeiras etapas de reconhecimento e validação da notificação do ciclo de vida são semelhantes a [responder a uma notificação de alteração de recursos](webhooks.md#processing-the-notification).

1. Aceite o recebimento da notificação respondendo a chamada POSTAGEM com `HTTP 202 Accepted`.
2. Validar a autenticidade da notificação. Mais detalhes [abaixo](#validating-the-authenticity-of-notifications).
3. Certifique-se de que o aplicativo tenha um token de acesso válido para a próxima etapa. 

    Se você estiver usando uma das [bibliotecas de autenticação](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), a biblioteca fará isso para você ao reutilizar um token de cache válido ou obtendo um novo token ao pedir ao usuário para fazer logon novamente com uma nova senha. Entretanto, a obtenção de um novo token pode falhar, pois as condições de acesso podem ser alteradas e o usuário não poderá mais acessar os dados de recursos.

4. Chamar uma das duas APIs a seguir. Se a chamada da API tiver êxito, o fluxo de notificação de recurso será retomado.

    - Chame a ação `/reauthorize` para autorizar novamente a assinatura sem estender a data de vencimento:
        ```http
        POST  https://graph.microsoft.com/beta/subscriptions/{id}/reauthorize
        Content-type: application/json
        ```
    - Execute uma ação de renovação regular para autorizar novamente e renova a assinatura ao mesmo tempo:
        ```http
        PATCH https://graph.microsoft.com/beta/subscriptions/{id}
        Content-Type: application/json

        {
           "expirationDateTime": "2019-09-21T11:00:00.0000000Z"
        }
        ```

      A renovação pode falhar, porque as verificações de autorização realizadas pelo sistema podem recusar o aplicativo ou o acesso do usuário ao recurso. Pode ser necessário que o aplicativo obtenha um novo token de acesso do usuário para autorizar novamente com êxito uma assinatura. 
      
      Você pode tentar essa ações mais tarde, a qualquer momento e obter êxito se as condições de acesso mudarem. Todas as notificações sobre as alterações de recursos que ocorrem entre o tempo de envio da notificação do ciclo de vida e o tempo em que o aplicativo eventualmente recria a assinatura com êxito, seriam perdidas. Nesses casos, o aplicativo deve buscar essas mudanças separadamente.

### <a name="tips"></a>Dicas 

Lembre-se do seguinte:

1. Os desafios de autorização não substituem a necessidade de renova uma assinatura de alteração de recursos antes de expirar. 

    Embora você possa optar por renovar uma assinatura quando recebe um desafio de autorização, o Microsoft Graph pode não desafiar todas as suas assinaturas. Por exemplo, uma assinatura que não tem atividade e não tem notificações de recursos com entrega pendente pode não sinalizar desafios de reautorização para o aplicativo. Certifique-se de [renovar assinaturas](webhooks.md#renewing-a-subscription) antes de expirarem.

2. A frequência dos desafios de autorização está sujeita a mudanças.

    Não faça suposições sobre a frequência dos desafios de autorização. Essas notificações informam quando executar ações, evitando que você tenha que acompanhar quais assinaturas devem ser autorizadas novamente. Esteja pronto para lidar com os desafios de autorização seja uma vez em alguns minutos para cada assinatura ou raramente para algumas das suas assinaturas.

### <a name="future-proof-your-code-to-handle-other-types-of-life-cycle-notifications"></a>Proteja o seu código para lidar com outros tipos de notificações do ciclo de vida

Espere que as notificações do ciclo de vida de assinatura sejam publicadas no mesmo ponto de extremidade especificado por **lifecycleNotificationUrl**. Elas são diferenciadas pela propriedade **lifecycleEvent** e podem conter um esquema e propriedades ligeiramente diferentes para atender aos cenários que resolvem.

Implemente seu código em antecipação dos novos tipos de notificações do ciclo de vida:

1. Use a propriedade **lifecycleEvent** para identificar o tipo de notificação para determinar a resposta adequada. Por exemplo, procure a `"lifecycleEvent": "reauthorizationRequired"` propriedade para identificar um evento específico e tratá-lo.

1. Registre todos os eventos do ciclo de vida que seu aplicativo não reconhece para obter conhecimento.

1. Inscreva-se no [Blog do Desenvolvedor do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) para assistir aos comunicados de notificações do ciclo de vida dos novos cenários.

1. Procure a documentação relacionada às novas notificações do ciclo de vida e implemente o suporte para elas conforme necessário.

## <a name="validating-the-authenticity-of-notifications"></a>Validar a autenticidade das notificações 

Os aplicativos geralmente executam lógica de negócios com base nos dados de recursos incluídos nas notificações. Verificar primeiro a autenticidade de cada notificação é importante. Caso contrário, um terceiro poderia simular seu aplicativo com notificações falsas, fazê-lo executa a lógica de negócios incorretamente e levar a um incidente de segurança.

Para obter notificações básicas que não contenham dados de recursos, basta validá-las com base no valor **clientState** conforme descrito [aqui](webhooks.md#processing-the-notification). Isso é aceitável, uma vez que você pode fazer chamadas confiáveis subsequentes do Microsoft Graph para obter acesso ao dados do recurso, portanto, o impacto das tentativas de falsificação é limitado. 

Para obter notificações que fornecem dados de recursos, realize uma validação mais completa antes de processar os dados.

Nesta seção:

- [Tokens de validação na notificação](#validation-tokens-in-the-notification)
- [Como validar](#how-to-validate)
- [Exemplo de token JWT](#example-jwt-token)

### <a name="validation-tokens-in-the-notification"></a>Tokens de validação na notificação

Uma notificação com dados de recursos contém uma propriedade adicional, **validationTokens**, que contém uma matriz de tokens JWT gerados pelo Microsoft Graph. O Microsoft Graph gera um único token para cada aplicativo distinto e par de locatários para os quais há um item na matriz **valor**. Lembre-se de que as notificações podem conter uma mistura de itens para vários aplicativos e locatários que se inscreveram usando os mesmo **notificationUrl**.

No exemplo a seguir, a notificação contém dois itens para o mesmo aplicativo e para dois locatários diferentes, portanto, a matriz **validationTokens** contém dois tokens que precisam ser validados.

```json
{
    "value": [
          {
            "subscriptionId": "76619225-ff6b-4489-96ca-4ef547e78b22",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
            "changeType": "created",
            ...
          },
      {
            "subscriptionId": "e990d58f-fd93-40af-acf7-a7c907c5d8ea",
      "tenantId": "46d9e3bd-6309-4177-a016-b256a411e30f",
            "changeType": "created",
            ...
            }
    ],
    "validationTokens": [
        "eyJ0eXAiOiJKV1QiLCJhb...",
    "cGlkYWNyIjoiMiIsImlkc..."
    ]
}
```
### <a name="how-to-validate"></a>Como validar

Se você não está familiarizado com a validação de tokens, confira este [artigo do blog](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/) para obter uma visão geral. Use um SDK, como o [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) da biblioteca da Microsoft para .NET ou uma biblioteca de terceiros para uma plataforma diferente.

Fique atento ao seguinte: 

- Certifique-se de sempre mandar um código de status `HTTP 202 Accepted` como parte da resposta à notificação. 
- Faça isso antes de validar a notificação (por exemplo, se você armazenar notificações em filas para processamento posterior) ou depois (se você as processar em tempo real), mesmo se a validação falhar.
- A aceitação de uma notificação evita tentativas de entrega desnecessárias e também impede que possíveis atores invasores descubram se passaram ou falharam na validação. Você sempre pode optar por ignorar uma notificação inválida após aceitá-la.

Especificamente, realize a validação em todos os tokens JWT na coleção **validationTokens**. Se os tokens falharem, considere a notificação como suspeita e continue investigando. 

Use as etapas a seguir para validar tokens e aplicativos que geram tokens:

1. Valide se o token não expirou.

2. Valide se o token não foi adulterado e foi emitido pela autoridade esperada, o Active Directory do Microsoft Azure:

    - Obtenha as chaves de assinatura do ponto de extremidade de configuração comum: `https://login.microsoftonline.com/common/.well-known/openid-configuration`. Essa configuração é armazenada em cache pelo aplicativo por um período de tempo. Lembre-se de que a configuração é atualizada frequentemente, uma vez que as chaves de assinatura são giradas diariamente.
    - Verifique a assinatura do token JWT usando essas chaves.

    Não aceite tokens emitidos por outra autoridade.

3. Valide se o token foi emitido para o aplicativo que está inscrito para alterar as notificações.

    As etapas a seguir fazem parte da lógica de validação padrão nas bibliotecas de token JWT e podem ser tipicamente executadas como uma única chamada de função. 
    - Valide a “audiência” no token que corresponde à ID do seu aplicativo.
    - Se você tiver mais de um aplicativo recebendo notificações, certifique-se de verificar várias IDs.


4. **Crítico**: valide se o aplicativo que gerou o token representa o distribuidor de notificação de alteração do Microsoft Graph. 

    - Verifique se a propriedade **appid** no token corresponde ao valor esperado de `0bf30f3b-4a52-48df-9a82-234910c4a086`.
    - Isso garante que as notificações não sejam enviadas por um aplicativo diferente que não seja o Microsoft Graph.


### <a name="example-jwt-token"></a>Exemplo de Token JWT 

Veja um exemplo das propriedades incluídas no token JWT que são necessárias para a validação:

```json
{
  // aud is your app's id 
  "aud": "8e460676-ae3f-4b1e-8790-ee0fb5d6148f",                           
  "iss": "https://sts.windows.net/84bd8158-6d4d-4958-8b9f-9d6445542f95/",
  "iat": 1565046813,
  "nbf": 1565046813,
  // Expiration date 
  "exp": 1565075913,                                                        
  "aio": "42FgYKhZ+uOZrHa7p+7tfruauq1HAA==",
  // appid represents the notification publisher and must always be the same value of 0bf30f3b-4a52-48df-9a82-234910c4a086 
  "appid": "0bf30f3b-4a52-48df-9a82-234910c4a086",                          
  "appidacr": "2",
  "idp": "https://sts.windows.net/84bd8158-6d4d-4958-8b9f-9d6445542f95/",
  "tid": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
  "uti": "-KoJHevhgEGnN4kwuixpAA",
  "ver": "1.0"
}
```

### <a name="example-verifying-validation-tokens"></a>Exemplo: verificação de tokens de validação

```csharp
// add Microsoft.IdentityModel.Protocols.OpenIdConnect and System.IdentityModel.Tokens.Jwt nuget packages to your project
public async Task<bool> ValidateToken(string token, string tenantId, IEnumerable<string> appIds)
{
    var configurationManager = new ConfigurationManager<OpenIdConnectConfiguration>("https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration", new OpenIdConnectConfigurationRetriever());
    var openIdConfig = await configurationManager.GetConfigurationAsync();
    var handler = new JwtSecurityTokenHandler();
    try
    {
    handler.ValidateToken(token, new TokenValidationParameters
    {
        ValidateIssuer = true,
        ValidateAudience = true,
        ValidateIssuerSigningKey = true,
        ValidateLifetime = true,
        ValidIssuer = $"https://sts.windows.net/{tenantId}/",
        ValidAudiences = appIds,
        IssuerSigningKeys = openIdConfig.SigningKeys
    }, out _);
    return true;
    }
    catch (Exception ex)
    {
    Trace.TraceError($"{ex.Message}:{ex.StackTrace}");
    return false;
    }
}
```
```java
private boolean IsValidationTokenValid(String[] appIds, String tenantId, String serializedToken) {
    try {
        JwkKeyResolver jwksResolver = new JwkKeyResolver();
        Jws<Claims> token = Jwts.parserBuilder()
        .setSigningKeyResolver(jwksResolver)
        .build()
        .parseClaimsJws(serializedToken);
        Claims body = token.getBody();
        String audience = body.getAudience();
        boolean isAudienceValid = false;
        for(String appId : appIds) {
        isAudienceValid = isAudienceValid || appId.equals(audience);
        }
        boolean isTenantValid = body.getIssuer().endsWith(tenantId + "/");
        return isAudienceValid  && isTenantValid; //nbf,exp and signature are already validated by library
    } catch (Exception e) {
        LOGGER.error("could not validate token");
        LOGGER.error(e.getMessage());
        return false;
    }
}
```
```JavaScript
import jwt from 'jsonwebtoken';
import jkwsClient from 'jwks-rsa';

const client = jkwsClient({
  jwksUri: 'https://login.microsoftonline.com/common/discovery/v2.0/keys'
});

export function getKey(header, callback) {
  client.getSigningKey(header.kid, (err, key) => {
    var signingKey = key.publicKey || key.rsaPublicKey;
    callback(null, signingKey);
  });
}

export function isTokenValid(token, appId, tenantId) {
  return new Promise((resolve) => {
    const options = {
      audience: [appId],
      issuer: [`https://sts.windows.net/${tenantId}/`]
    };
    jwt.verify(token, getKey, options, (err) => {
      if (err) {
        // eslint-disable-next-line no-console
        console.error(err);
        resolve(false);
      } else {
        resolve(true);
      }
    });
  });
}
```
Para que o exemplo do Java funcione, também será necessário implementar o `JwkKeyResolver`.  
```java
package com.example.restservice;

import com.auth0.jwk.JwkProvider;
import com.auth0.jwk.UrlJwkProvider;
import com.auth0.jwk.Jwk;
import io.jsonwebtoken.Claims;
import io.jsonwebtoken.JwsHeader;
import io.jsonwebtoken.SigningKeyResolverAdapter;
import java.security.Key;
import java.net.URI;
import org.slf4j.Logger;
import org.slf4j.LoggerFactory;

public class JwkKeyResolver extends SigningKeyResolverAdapter {
    private JwkProvider keyStore;
    private final Logger LOGGER = LoggerFactory.getLogger(this.getClass());
    public JwkKeyResolver() throws java.net.URISyntaxException, java.net.MalformedURLException {
        this.keyStore = new UrlJwkProvider((new URI("https://login.microsoftonline.com/common/discovery/keys").toURL()));
    }
    @Override
    public Key resolveSigningKey(JwsHeader jwsHeader, Claims claims) {
        try {
            String keyId = jwsHeader.getKeyId();
            Jwk pub = keyStore.get(keyId);
            return pub.getPublicKey();
        } catch (Exception e) {
            LOGGER.error(e.getMessage());
            return null;
        }
    }
}
```

## <a name="decrypting-resource-data-from-change-notifications"></a>Descriptografar os dados de recursos de notificações de alteração

A propriedade **resourceData** de uma notificação inclui apenas as informações de ID básico e tipo de uma instância de recurso. A propriedade **encryptedData** contém os dados de recursos completos, criptografados pelo Microsoft Graph usando a chave pública fornecida na assinatura. A propriedade também contém valores necessários para verificação e descriptografia. Isso é feito para aumentar a segurança dos dados do cliente acessados através de notificações. É a sua responsabilidade proteger a chave privada para garantir que os dados do cliente não possam ser descriptografados por terceiros, mesmo que eles consigam interceptar as notificações originais.

Nesta seção:

- [Gerenciar as chaves de criptografia](#managing-encryption-keys)
- [Descriptografar os dados de recursos](#decrypting-resource-data)
- [Exemplo: descriptografar uma notificação com dados de recursos criptografados](#example-decrypting-a-notification-with-encrypted-resource-data)

### <a name="managing-encryption-keys"></a>Gerenciar as chaves de criptografia

1. Obtenha um certificado com um par de chaves assimétricas.

    - Você pode assinatura o certificado sozinho, uma vez que o Microsoft Graph não verifica o emissor do certificado e usa a chave pública somente para criptografia. 
    - Use o [Cofre da Chave do Azure](https://docs.microsoft.com/azure/key-vault/key-vault-whatis) como a solução para criar, girar e gerenciar certificados com segurança. Cerifique-se de que as chaves atendem aos seguintes critérios:

        - A chave deve ser do tipo `RSA`
        - O tamanho da chave deve estar entre 2048 e 4096 bits

2. Exportar o certificar no formato base64-encoded X.509 e **incluir apenas a chave pública**. 

3. Ao criar uma assinatura:

    - Forneça o certificado na propriedade **encryptionCertificate** usando o conteúdo base64-encoded no qual o certificado foi exportado.
    - Forneça seu próprio identificador na propriedade **encryptionCertificateId**. 
  
        Esse identificador permite que você combine seus certificados com as notificações recebidas e que você recupere os certificados do seu repositório de certificados. O identificador pode ter no máximo 128 caracteres.

4. Gerencie a chave privada de forma segura para que seu código de processamento de notificação possa acessar a chave privada para descriptografar os dados de recursos.

#### <a name="rotating-keys"></a>Chaves de rotação

Para minimizar o risco de uma chave privada ser comprometida, altere periodicamente suas chaves assimétricas. Siga estas etapas para introduzir um novo par de chaves:

1. Obtenha um novo certificado com um novo par de chaves assimétricas. Use-o para todas as novas assinaturas sendo criadas.

2. Atualize as assinaturas existentes com a nova chave de certificado.

    - Faça isso como parte da renovação da assinatura regular. 
    - Ou enumere todas as assinaturas e forneça a chave. Use a [operação PATCH na assinatura](/graph/api/subscription-update?view=graph-rest-1.0) e atualize as propriedades **encryptionCertificate** e **encryptionCertificateId**.

3. Lembre-se do seguinte:
    - Por um período de tempo, o certificado antigo ainda pode ser usado para criptografia. Seu aplicativo deve ter acesso a certificados novos e antigos para poder descriptografar o conteúdo.
    - Use a propriedade **encryptionCertificateId** em cada notificação para identificar a chave correta a ser usada.
    - Descarte o certificado antigo somente quando não tiver visto nenhuma notificação recente referenciando-o.

### <a name="decrypting-resource-data"></a>Descriptografar dados de recursos

Para otimizar o desempenho, o Microsoft Graph usa um processo de criptografia de duas etapas:
  - Ele gera uma chave simétrica de uso único e a usa para criptografar os dados do recurso.
  - Ele usa a chave pública assimétrica (que você forneceu ao se inscrever) para criptografar a chave simétrica e inclui-la em cada notificação dessa assinatura.

Presuma sempre que a chave simétrica é diferente para cada item na notificação.

Para descriptografar os dados do recurso, seu aplicativo deve executar as etapas inversas usando as propriedades em **encryptedContent** em cada notificação:

1. Use a propriedade **encryptionCertificateId** para identificar o certificado a ser usado.

2. Inicialize um componente criptográfico da RSA (como o .NET [RSACryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)) com a chave privada.

3. Descriptografe a chave simétrica entregue na propriedade **dataKey** de cada item na notificação.

    Use o Preenchimento de Criptografia Assimétrica Ideal (OAEP) para o algoritmo de descriptografia.

4. Use a chave simétrica para calcular a assinatura HMAC-SHA256 do valor em **dados**.
  
    Compare-o com o valor em **dataSignature**. Se eles não corresponderem, considere que a carga foi adulterada e não a descriptografe.

5. Use a chave simétrica com a criptografia AES (como o .NET [AesCryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)) para descriptografar o conteúdo em **dados**.

    - Use os seguintes parâmetros de descriptografia para o algoritmo AES:

        - Preenchimento: PKCS7
        - Modo de criptografia: CBC
    - Defina o “vetor de inicialização” copiando os primeiros 16 bytes da chave simétrica usada para descriptografia.

6. O valor descriptografado é uma cadeia de caracteres JSON que representa a instância do recurso na notificação.


### <a name="example-decrypting-a-notification-with-encrypted-resource-data"></a>Exemplo: descriptografar uma notificação com dados de recurso criptografados

Veja a seguir um exemplo de notificação que inclui valores de propriedade criptografados de uma instância **chatMessage** em uma mensagem do canal. A instância é especificada pelo valor `@odata.id`.

```json
{
    "value": [
        {
            "subscriptionId": "76222963-cc7b-42d2-882d-8aaa69cb2ba3",
            "changeType": "created",
            // Other properties typical in a resource change notification
            "resource": "teams('d29828b8-c04d-4e2a-b2f6-07da6982f0f0')/channels('19:f127a8c55ad949d1a238464d22f0f99e@thread.skype')/messages('1565045424600')/replies('1565047490246')",
            "resourceData": {
                "id": "1565293727947",
                "@odata.type": "#Microsoft.Graph.ChatMessage",
                "@odata.id": "teams('88cbc8fc-164b-44f0-b6a6-b59b4a1559d3')/channels('19:8d9da062ec7647d4bb1976126e788b47@thread.tacv2')/messages('1565293727947')/replies('1565293727947')"
            },
            "encryptedContent": {
                "data": "{encrypted data that produces a full resource}",
        "dataSignature": "<HMAC-SHA256 hash>",
                "dataKey": "{encrypted symmetric key from Microsoft Graph}",
                "encryptionCertificateId": "MySelfSignedCert/DDC9651A-D7BC-4D74-86BC-A8923584B0AB",
                "encryptionCertificateThumbprint": "07293748CC064953A3052FB978C735FB89E61C3D"
            }
        }
    ],
    "validationTokens": [
        "eyJ0eXAiOiJKV1QiLCJhbGciOiJSU..."
    ]
}
```

A seção contém alguns trechos de código úteis que usam C# e .NET em cada etapa da descriptografia.

#### <a name="decrypt-the-symmetric-key"></a>Descriptografar a chave simétrica

```csharp
// Initialize with the private key that matches the encryptionCertificateId.
RSACryptoServiceProvider rsaProvider = ...;        
byte[] encryptedSymmetricKey = Convert.FromBase64String(<value from dataKey property>);

// Decrypt using OAEP padding.
byte[] decryptedSymmetricKey = rsaProvider.Decrypt(encryptedSymmetricKey, fOAEP: true);

// Can now use decryptedSymmetricKey with the AES algorithm.
```
```Java
String storename = ""; //name/path of the jks store
String storepass = ""; //password used to open the jks store
String alias = ""; //alias of the certificate when store in the jks store, should be passed as encryptionCertificateId when subscribing and retrieved from the notification
KeyStore ks = KeyStore.getInstance("JKS");
ks.load(new FileInputStream(storename), storepass.toCharArray());
Key asymmetricKey = ks.getKey(alias, storepass.toCharArray());
byte[] encryptedSymetricKey = Base64.decodeBase64("<value from dataKey property>");
Cipher cipher = Cipher.getInstance("RSA/ECB/OAEPWithSHA1AndMGF1Padding");
cipher.init(Cipher.DECRYPT_MODE, asymmetricKey);
byte[] decryptedSymmetricKey = cipher.doFinal(encryptedSymetricKey);
// Can now use decryptedSymmetricKey with the AES algorithm.
```
```JavaScript
const base64encodedKey = 'base 64 encoded dataKey value';
const asymetricPrivateKey = 'pem encoded private key';
const decodedKey = Buffer.from(base64encodedKey, 'base64');
const decryptedSymetricKey = crypto.privateDecrypt(asymetricPrivateKey, decodedKey);
// Can now use decryptedSymmetricKey with the AES algorithm.
```

#### <a name="compare-data-signature-using-hmac-sha256"></a>Comparar assinatura de dados usando HMAC-SHA256

```csharp
byte[] decryptedSymmetricKey = <the aes key decrypted in the previous step>;
byte[] encryptedPayload = <the value from the data property, still encrypted>;
byte[] expectedSignature = <the value from the dataSignature property>;
byte[] actualSignature;

using (HMACSHA256 hmac = new HMACSHA256(decryptedSymmetricKey))
{
    actualSignature = hmac.ComputeHash(encryptedPayload);
}
if (actualSignature.SequenceEqual(expectedSignature))
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```
```Java
byte[] decryptedSymmetricKey = "<the aes key decrypted in the previous step>";
byte[] decodedEncryptedData = Base64.decodeBase64("data property from encryptedContent object");
Mac mac = Mac.getInstance("HMACSHA256");
SecretKey skey = new SecretKeySpec(decryptedSymmetricKey, "HMACSHA256");
mac.init(skey);
byte[] hashedData = mac.doFinal(decodedEncryptedData);
String encodedHashedData = new String(Base64.encodeBase64(hashedData));
if (comparisonSignature.equals(encodedHashedData))
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```
```JavaScript
const decryptedSymetricKey = []; //Buffer provided by previous step
const base64encodedSignature = 'base64 encodded value from the dataSignature property';
const hmac = crypto.createHmac('sha256', decryptedSymetricKey);
hmac.write(base64encodedPayload, 'base64');
if(base64encodedSignature === hmac.digest('base64'))
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```

#### <a name="decrypt-the-resource-data-content"></a>Descriptografar o conteúdo dos dados de recursos

```csharp
AesCryptoServiceProvider aesProvider = new AesCryptoServiceProvider();
aesProvider.Key = decryptedSymmetricKey;
aesProvider.Padding = PaddingMode.PKCS7;
aesProvider.Mode = CipherMode.CBC;

// Obtain the intialization vector from the symmetric key itself.
int vectorSize = 16;
byte[] iv = new byte[vectorSize];
Array.Copy(decryptedSymmetricKey, iv, vectorSize);
aesProvider.IV = iv;

byte[] encryptedPayload = Convert.FromBase64String(<value from dataKey property>);

string decryptedResourceData;
// Decrypt the resource data content.
using (var decryptor = aesProvider.CreateDecryptor())
{
  using (MemoryStream msDecrypt = new MemoryStream(encryptedPayload))
  {
      using (CryptoStream csDecrypt = new CryptoStream(msDecrypt, decryptor, CryptoStreamMode.Read))
      {
          using (StreamReader srDecrypt = new StreamReader(csDecrypt))
          {
              decryptedResourceData = srDecrypt.ReadToEnd();
          }
      }
  }
}

// decryptedResourceData now contains a JSON string that represents the resource.
```
```Java
SecretKey skey = new SecretKeySpec(decryptedSymmetricKey, "AES");
IvParameterSpec ivspec = new IvParameterSpec(Arrays.copyOf(decryptedSymmetricKey, 16));
Cipher cipher = Cipher.getInstance("AES/CBC/PKCS5PADDING");
cipher.init(Cipher.DECRYPT_MODE, skey, ivspec);
String decryptedResourceData = new String(cipher.doFinal(Base64.decodeBase64(encryptedData)));
```
```JavaScript
const base64encodedPayload = 'base64 encoded value from data property';
const decryptedSymetricKey = []; //Buffer provided by previous step
const iv = Buffer.alloc(16, 0);
decryptedSymetricKey.copy(iv, 0, 0, 16);
const decipher = crypto.createDecipheriv('aes-256-cbc', decryptedSymetricKey, iv);
let decryptedPayload = decipher.update(base64encodedPayload, 'base64', 'utf8');
decryptedPayload += decipher.final('utf8');
```

## <a name="see-also"></a>Confira também

- [Configurar notificações para alterações nos dados de usuário](webhooks.md)
- [Tipo de recurso de assinatura](/graph/api/resources/subscription?view=graph-rest-beta)
- [Obter assinatura](/graph/api/subscription-get?view=graph-rest-1.0)
- [Criar assinatura](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [Atualizar assinatura](/graph/api/subscription-update?view=graph-rest-1.0)
