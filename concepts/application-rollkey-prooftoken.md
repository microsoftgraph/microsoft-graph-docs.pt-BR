---
title: Gerando um token de comprovação de posse para sobrepor chaves
description: Como parte da validação da solicitação para os métodos addKey e removeKey, é necessário um token de comprovação de posse. Este documento fornece orientação para gerar o token de comprovação de posse.
ms.localizationpriority: high
ms.prod: applications
author: FaithOmbongi
ms.openlocfilehash: 495c0a86020ff463b0bb76ab89f4f6b367e3af8d
ms.sourcegitcommit: 6a4e81d2b8e7447771c9060998c7e1cc18a57902
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/03/2022
ms.locfileid: "66609651"
---
# <a name="generating-proof-of-possession-tokens-for-rolling-keys"></a>Gerando um token de comprovação de posse para sobrepor chaves

Você pode usar os métodos **addKey** e **removeKey** definidos no [aplicativo](/graph/api/resources/application) e recursos [servicePrincipal](/graph/api/resources/serviceprincipal) para acumular as chaves expiradas por programação.

Como parte da solicitação de validação para esses métodos, uma comprovação de posse de uma chave existente é verificada antes que os métodos possam ser invocados. As comprovações são representadas por um token JWT autoassinado. Esse token de JWT deve ser assinado usando a chave privada de um dos certificados válidos existentes do aplicativo. O tempo de vida do token não deve exceder 10 minutos.

> **Observação:** Aplicativos que não têm certificados válidos existentes (nenhum certificado foi adicionado ainda, ou todos os certificados expiraram), não poderão usar essa ação de serviço. Você pode usar a operação [Atualizar aplicativo](/graph/api/application-update) para executar uma atualização.

O token deve conter os seguintes argumentos:

- `aud` – A audiência deve ser `00000002-0000-0000-c000-000000000000`.
- `iss` – O emissor deve ser o Azure AD __ObjectId__  do aplicativo que está fazendo a chamada (não é o applicationId ou o clientId).
- `nbf` – Não antes da hora.
- `exp` – O tempo de expiração deve ser "nbf" + 10 min.

Você pode usar o seguinte exemplo de código para gerar esse token de comprovação de posse.

```csharp
using System;
using System.Collections.Generic;
using System.Security.Cryptography.X509Certificates;
using Microsoft.IdentityModel.Tokens;
using Microsoft.IdentityModel.JsonWebTokens;

namespace MicrosoftIdentityPlatformProofTokenGenerator
{
    class Program
    {
        static void Main(string[] args)
        {
            // Configure the following
            string pfxFilePath = "<Path to your certificate file";
            string password = "<Certificate password>";
            string objectId = "<id of the application or servicePrincipal object>";

            // Get signing certificate
            X509Certificate2 signingCert = new X509Certificate2(pfxFilePath, password);

            // audience
            string aud = $"00000002-0000-0000-c000-000000000000";

            // aud and iss are the only required claims.
            var claims = new Dictionary<string, object>()
            {
                { "aud", aud },
                { "iss", objectId }
            };

            // token validity should not be more than 10 minutes
            var now = DateTime.UtcNow;
            var securityTokenDescriptor = new SecurityTokenDescriptor
            {
                Claims = claims,
                NotBefore = now,
                Expires = now.AddMinutes(10),
                SigningCredentials = new X509SigningCredentials(signingCert)
            };

            var handler = new JsonWebTokenHandler();
            var x = handler.CreateToken(securityTokenDescriptor);
            Console.WriteLine(x);
        }
    }
}
```

> **Observação:** a prova pode ser gerada usando outras ferramentas, como o PowerShell ou a assinatura usando o Azure KeyVault. É importante observar que o caractere de preenchimento “=” não deve ser incluído no cabeçalho e na carga JWT, ou um erro **Authentication_MissingOrMalformed** será retornado.
