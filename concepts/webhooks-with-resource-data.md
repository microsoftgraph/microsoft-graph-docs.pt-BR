---
title: Configurar notificações de alteração que incluam dados de recurso
description: O Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. As notificações de alteração podem incluir propriedades de recursos.
author: Jumaodhiss
ms.prod: non-product-specific
ms.localizationpriority: high
ms.openlocfilehash: d13db88f179bbce58a6d45fa567b507199fa95f8
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337058"
---
# <a name="set-up-change-notifications-that-include-resource-data"></a>Configurar notificações de alteração que incluam dados de recurso

O Microsoft Graph permite que os aplicativos inscrevam-se para alterar as notificações de recursos através do [webhooks](webhooks.md). É possíve configurar as assinaturas para incluir os dados alterados dos recursos (como o conteúdo de uma mensagem de bate-papo ou informações de presença do Microsoft Teams) nas notificações de alteração. Em seguida, seu aplicativo pode usar a lógica de negócios sem ter que fazer uma chamada à API separada para buscar o recurso alterado. Como resultado, o aplicativo funciona melhor ao realizar menos chamadas da API, o que é benéfico em cenários de larga escala.

A inclusão de dados de recursos como parte das notificações de alteração exige que, para atender aos requisitos de acesso e segurança de dados, você implemente a seguinte lógica adicional : 

- [Lide](webhooks-lifecycle.md#responding-to-reauthorizationrequired-notifications) com notificações de ciclo de vida de assinatura especial para manter um fluxo ininterrupto de dados. O Microsoft Graph envia notificações sobre o ciclo de vida de tempos em tempos para exigir que um aplicativo seja autorizado novamente e para garantir que os problemas de acesso não ocorram inesperadamente, incluindo dados de recursos nas notificações de alterações.
- [Confirme](#validating-the-authenticity-of-notifications) a autenticidade das notificações de alteração como originárias do Microsoft Graph.
- [Forneça](#decrypting-resource-data-from-change-notifications) uma chave de criptografia pública e utilize uma chave privada para decriptar os dados de recursos recebidos por meio das notificações de alteração.

## <a name="resource-data-in-notification-payload"></a>Dados de recursos na carga de notificação 

Geralmente, esse tipo de notificação de alteração inclui os seguintes dados de recursos na carga:

- ID e tipo de instância de recurso alterado, retornados na propriedade **resourceData**.
- Todos os valores de propriedade da instância de recurso, criptografados conforme especificado na assinatura, retornados na propriedade **encryptedContent**.
- Or, dependendo do recurso, propriedades específicas retornadas na propriedade **resourceData**. Para obter somente propriedades específicas, especifique-as como parte da URL do **recurso** na assinatura, usando um parâmetro `$select`.  


## <a name="supported-resources"></a>Recursos com suporte

Os recursos do Microsoft Teams [chatMessage](/graph/api/resources/chatmessage) e [presença](/graph/api/resources/presence)suportam notificações de alteração com dados de recursos. Os [outlook](/graph/api/resources/contact.md), [eventos](/graph/api/resources/event.md), [mensagem](/graph/api/resources/message.md) recursos têm suporte semelhante _na visualização_. Especificamente, você pode configurar uma assinatura para os casos de uso listados abaixo.

Disponível nos pontos de extremidade v1.0 e beta:
- Mensagens novas ou alteradas em um canal específico do Teams: `/teams/{id}/channels/{id}/messages`
- Mensagens novas ou alteradas em todos os canais do Teams em toda a organização (locatário): `/teams/getAllMessages`
- Mensagens novas ou alteradas em um bate-papo específico do Teams: `/chats/{id}/messages`
- Mensagens novas ou alteradas em todos os bate-papos em toda a organização (locatário): `/chats/getAllMessages`
- Atualização das informações de presença do usuário: `/communications/presences/{id}`

Disponível apenas no ponto de extremidade beta:
- Contatos pessoais novos ou alterados na caixa de correio de um usuário: `/users/{id}/contacts`
- Contatos pessoais novos ou alterados no contactFolder de um usuário: `/users/{id}/contactFolders/{id}/contacts`
- Eventos novos ou alterados na caixa de correio de um usuário: `/users/{id}/events`
- Mensagens novas ou alteradas na caixa de correio de um usuário: `/users/{id}/messages`
- Mensagens novas ou alteradas na mailFolder de um usuário: `/users/{id}/mailFolders/{id}/messages`

As notificações de alteração que incluem **chatMessage** ou dados de recursos de **presença** consistem em todas as propriedades da instância alterada. Eles não dão suporte ao retorno apenas das propriedades selecionadas da instância. 

As notificações de alteração para os recursos **contato**, **evento**, ou de **mensagem** incluem apenas um subconjunto de propriedades para o recurso, que deve ser especificado na solicitação de assinatura correspondente usando um parâmetro de consulta `$select`. Para obter mais informações e um exemplo de assinatura para alterar notificações com dados de recurso para o recurso de **mensagem**, consulte [Alterar notificações para Outlook recursos no Microsoft Graph](outlook-change-notifications-overview.md). 

O restante deste artigo explica um exemplo para assinar notificações de alteração para recursos **chatMessage** em um canal do Teams, com cada notificação de alteração, incluindo os dados completos de recursos da instância **chatMessage** alterada. Para obter mais detalhes sobre assinaturas baseadas em **chatMessage**, confira [Obter notificações de alteração para mensagens de chat e canal](teams-changenotifications-chatmessage.md).

## <a name="creating-a-subscription"></a>Criar uma assinatura

Para que os dados de recursos estejam incluídos nas notificações de alteração, você **deve** especificar as seguintes propriedades, além das que geralmente são especificadas ao [criar uma assinatura](webhooks.md#creating-a-subscription):

- **includeResourceData** que deve ser definido como `true` para solicitar explicitamente os dados de recursos.
- **encryptionCertificate** que contém apenas a chave público que o Microsoft Graph usa para criptografar os dados de recursos. Mantenha a chave privada correspondente para [descriptografar o conteúdo](#decrypting-resource-data-from-change-notifications).
- **encryptionCertificateId** é o seu próprio identificador para o certificado. Use esse ID para corresponder a cada notificação de alteração cujo certificado foi utilizado para descriptografia.

Lembre-se do seguinte:

- Valide os dois pontos de extremidade conforme descrito em [validação de ponto de extremidade de notificação](webhooks.md#notification-endpoint-validation). Se você optar por usar a mesma URL para ambos os pontos de extremidade, receberá e responderá a duas solicitações de validação.

### <a name="subscription-request-example"></a>Exemplo de solicitação de assinatura

O exemplo a seguir assina as mensagens de canal que estão sendo criadas ou atualizadas no Microsoft Teams.

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
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
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificateId": "{custom ID}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secret client state}"
}
```

## <a name="subscription-lifecycle-notifications"></a>Notificações do ciclo de vida da assinatura

Certos eventos podem interferir no fluxo de notificação de alterações em uma assinatura existente. As notificações sobre o ciclo de vida da assinatura informam as ações a serem tomadas para manter um fluxo ininterrupto. Ao contrário de uma notificação de alteração de recurso que informa uma alteração em uma instância de recurso, uma notificação do ciclo de vida é sobre a própria assinatura e seu estado atual no ciclo de vida. 

Para obter mais informações sobre como receber e responder a notificações de ciclo de vida, consulte [Reduzir assinaturas ausentes e notificações de alteração)](webhooks-lifecycle.md)

## <a name="validating-the-authenticity-of-notifications"></a>Validando a autenticidade das notificações

Os aplicativos geralmente executam a lógica comercial com base nos dados de recursos incluídos nas notificações de alterações. Verificar a autenticidade de cada notificação de alteração primeiro é importante. Caso contrário, um terceiro poderá imitar seu aplicativo com notificações de alteração falsa e fazê-lo executar a lógica de negócios incorretamente, e isso pode levar a um incidente de segurança.

Para notificações básicas de alterações que não contêm dados de recursos, simplesmente valide-as com base no valor **clientState** conforme descrito em [Processando a notificação de alteração](webhooks.md#processing-the-change-notification). Isso é aceitável, uma vez que você pode fazer chamadas confiáveis subsequentes do Microsoft Graph para obter acesso ao dados do recurso, portanto, o impacto das tentativas de falsificação é limitado. 

Para notificações de alteração que entregam dados de recursos, execute uma validação mais completa antes de processar os dados.

Nesta seção:

- [Tokens de validação na notificação de alteração](#validation-tokens-in-the-change-notification)
- [Como validar](#how-to-validate)
- [Exemplo de token JWT](#example-jwt-token)

### <a name="validation-tokens-in-the-change-notification"></a>Tokens de validação na notificação de alteração

Uma notificação de alteração com os dados do recurso contém uma propriedade adicional, **validationTokens**, com uma matriz de tokens JWT gerados pelo Microsoft Graph. O Microsoft Graph gera um token único para cada aplicativo distinto e um par de locatários onde existe um item no conunto **valor**. Tenha em mente que as notificações de alterações podem conter uma mistura de itens para vários aplicativos e locatários que fizeram assinatura usando o mesmo **notificationUrl**.

> **Observação:** se você estiver configurando notificações de alteração [entregues por meio do Hubs de Eventos do Azure](change-notifications-delivery.md), o Microsoft Graph não enviará os tokens de validação. Microsoft Graph não precisa validar o **notificationUrl**.


No exemplo a seguir, a notificação de alteração contém dois itens para o mesmo aplicativo e para dois locatários diferentes, portanto, o conjunto **validationTokens** contém dois tokens que precisam ser validados.

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

> **Nota:** para obter uma descrição completa dos dados enviados quando as notificações de alterações são entregues, consulte [ changeNotificationCollection](/graph/api/resources/changenotificationcollection).

### <a name="how-to-validate"></a>Como validar

Se você não conhece a validação de token, consulte [Princípios de Validação de Token](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/) para obter uma visão geral. Use um SDK, como a [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) biblioteca para .NET ou uma biblioteca de terceiros para uma plataforma diferente.

Fique atento ao seguinte: 

- Certifique-se de sempre enviar um `HTTP 202 Accepted` código de status como parte da resposta à notificação de alteração. 
- Responda antes de validar a notificação de alteração (por exemplo, se você armazenar as notificações de alteração em filas para processamento posterior) ou depois (se você as processar instantaneamente), mesmo se a validação falhar.
- A aceitação de uma notificação de alteração evita novas tentativas desnecessárias de entrega e também impede que possíveis atores invasores descubram se foram ou não aprovados na validação. Você sempre pode optar por ignorar uma notificação de alteração inválida após aceitá-la.

Especificamente, realize a validação em todos os tokens JWT na coleção **validationTokens**. Se algum token falhar, considere a notificação de alteração suspeita e investigue mais. 

Use as etapas a seguir para validar tokens e aplicativos que geram tokens:

1. Valide se o token não expirou.

2. Valide se o token não foi adulterado e foi emitido pela autoridade esperada, plataforma de identidade da Microsoft:

    - Obtenha as chaves de assinatura do ponto de extremidade de configuração comum: `https://login.microsoftonline.com/common/.well-known/openid-configuration`. Essa configuração é armazenada em cache pelo aplicativo por um período de tempo. Lembre-se de que a configuração é atualizada frequentemente, uma vez que as chaves de assinatura são giradas diariamente.
    - Verifique a assinatura do token JWT usando essas chaves.

    Não aceite tokens emitidos por outra autoridade.

3. Valide se o token foi emitido para o aplicativo que está inscrito para alterar as notificações.

    As etapas a seguir fazem parte da lógica de validação padrão nas bibliotecas de token JWT e podem ser tipicamente executadas como uma única chamada de função. 
    - Valide a “audiência” no token que corresponde à ID do seu aplicativo.
    - Se você tiver mais de um aplicativo recebendo notificações de alterações, verifique a existencia de vários IDs.


4. **Crítico**: valide se o aplicativo que gerou o token representa o distribuidor de notificação de alteração do Microsoft Graph. 

    - Verifique se a propriedade **appid** no token corresponde ao valor esperado de `0bf30f3b-4a52-48df-9a82-234910c4a086`.
    - Isso garante que as notificações de alteração não sejam enviadas por um aplicativo diferente do Microsoft Graph.


### <a name="example-jwt-token"></a>Exemplo de Token JWT 

A seguir, é apresentado um exemplo das propriedades incluídas no token JWT que são necessárias para validação.

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

A propriedade **resourceData** de uma notificação de alteração inclui apenas o ID básico e as informações do tipo de uma instância de recurso. A propriedade **encryptedData** contém os dados de recursos completos, criptografados pelo Microsoft Graph usando a chave pública fornecida na assinatura. A propriedade também contém valores necessários para verificação e descriptografia. Isso é feito para aumentar a segurança dos dados do cliente acessados por meio de notificações de alterações. É da sua responsabilidade proteger a chave privada para garantir que os dados do cliente não sejam decriptados por terceiros, mesmo que eles consigam interceptar as notificações de alteração originais.

Nesta seção:

- [Gerenciar as chaves de criptografia](#managing-encryption-keys)
- [Descriptografar os dados de recursos](#decrypting-resource-data)
- [Exemplo: descriptografar uma notificação com dados de recursos criptografados](#example-decrypting-a-notification-with-encrypted-resource-data)

### <a name="managing-encryption-keys"></a>Gerenciar as chaves de criptografia

1. Obtenha um certificado com um par de chaves assimétricas.

    - Você pode assinatura o certificado sozinho, uma vez que o Microsoft Graph não verifica o emissor do certificado e usa a chave pública somente para criptografia. 
    - Use o [Cofre da Chave do Azure](/azure/key-vault/key-vault-whatis) como a solução para criar, girar e gerenciar certificados com segurança. Cerifique-se de que as chaves atendem aos seguintes critérios:

        - A chave deve ser do tipo `RSA`
        - O tamanho da chave deve estar entre 2048 e 4096 bits

2. Exportar o certificar no formato base64-encoded X.509 e **incluir apenas a chave pública**. 

3. Ao criar uma assinatura:

    - Forneça o certificado na propriedade **encryptionCertificate** usando o conteúdo base64-encoded no qual o certificado foi exportado.
    - Forneça seu próprio identificador na propriedade **encryptionCertificateId**. 
  
        Esse identificador permite corresponder seus certificados às notificações de alterações recebidas e recuperar certificados do seu repositório de certificados. O identificador pode ter até 128 caracteres.

4. Gerencie com segurança a chave privada com para que seu código de processamento de notificação de alteração acesse a chave privada para decriptar os dados do recurso.

#### <a name="rotating-keys"></a>Chaves de rotação

Para minimizar o risco de uma chave privada ser comprometida, altere periodicamente suas chaves assimétricas. Siga estas etapas para introduzir um novo par de chaves:

1. Obtenha um novo certificado com um novo par de chaves assimétricas. Use-o para todas as novas assinaturas sendo criadas.

2. Atualize as assinaturas existentes com a nova chave de certificado.

    - Faça isso como parte da renovação da assinatura regular. 
    - Ou enumere todas as assinaturas e forneça a chave. Use a [operação PATCH na assinatura](/graph/api/subscription-update) e atualize as propriedades **encryptionCertificate** e **encryptionCertificateId**.

3. Lembre-se do seguinte:
    - Por um período de tempo, o certificado antigo ainda pode ser usado para criptografia. Seu aplicativo deve ter acesso a certificados novos e antigos para poder descriptografar o conteúdo.
    - Use a propriedade **encryptionCertificateId** em cada notificação de alteração para identificar a chave correta a ser utilizada.
    - Descarte o certificado antigo somente quando não houver notificações de alterações recentes fazendo referência a ele.

### <a name="decrypting-resource-data"></a>Descriptografar dados de recursos

Para otimizar o desempenho, o Microsoft Graph usa um processo de criptografia de duas etapas:
  - Ele gera uma chave simétrica de uso único e a usa para criptografar os dados do recurso.
  - Ele usa a chave pública assimétrica (que você forneceu ao fazer a assinatura) para criptografar a chave simétrica e a incluir em cada notificação de alteração desta assinatura.

Sempre assuma que a chave simétrica é diferente para cada item na notificação de alteração.

Para decriptar os dados de recursos, o seu aplicativo deve executar as etapas inversas, usando as propriedades **encryptedContent** em cada notificação de alteração:

1. Use a propriedade **encryptionCertificateId** para identificar o certificado a ser usado.

2. Inicialize um componente criptográfico da RSA (como o .NET [RSACryptoServiceProvider](/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8&preserve-view=true)) com a chave privada.

3. Decripte a chave simétrica entregue na propriedade **dataKey** de cada item na notificação de alteração.

    Use o Preenchimento de Criptografia Assimétrica Ideal (OAEP) para o algoritmo de descriptografia.

4. Use a chave simétrica para calcular a assinatura HMAC-SHA256 do valor em **dados**.
  
    Compare-o com o valor **dataSignature**. Se eles não corresponderem, suponha que a carga foi violada e não a descriptografe.

5. Use a chave simétrica com a criptografia AES (como o .NET [AesCryptoServiceProvider](/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8&preserve-view=true)) para descriptografar o conteúdo em **dados**.

    - Use os seguintes parâmetros de descriptografia para o algoritmo AES:

        - Preenchimento: PKCS7
        - Modo de criptografia: CBC
    - Defina o “vetor de inicialização” copiando os primeiros 16 bytes da chave simétrica usada para descriptografia.

6. O valor decriptado é uma sequência JSON que representa a instância do recurso na notificação de alteração.


### <a name="example-decrypting-a-notification-with-encrypted-resource-data"></a>Exemplo: decriptando uma notificação com dados de recurso criptografados

A seguir está um exemplo de notificação de alteração que inclui valores de propriedade criptografados de uma instância **chatMessage** em uma mensagem de canal. A instância é especificada pelo valor `@odata.id`.

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

> **Nota:** para obter uma descrição completa dos dados enviados quando as notificações de alterações são entregues, consulte [ changeNotificationCollection](/graph/api/resources/changenotificationcollection).


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
- [Tipo de recurso de assinatura](/graph/api/resources/subscription)
- [Obter assinatura](/graph/api/subscription-get)
- [Criar assinatura](/graph/api/subscription-post-subscriptions)
- [Atualizar assinatura](/graph/api/subscription-update)
- [Alterar notificações para recursos do Outlook no Microsoft Graph](outlook-change-notifications-overview.md)
