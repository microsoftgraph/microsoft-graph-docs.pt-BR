---
title: Geração de tokens de prova de posse para chaves de rolagem
description: Como parte da validação de solicitação para os métodos addKey e removeKey, um token de prova de posse é necessário. Este documento fornece orientações para gerar o token de prova de posse.
localization_priority: Priority
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 516673b3f5ef318f1c2cc42778d8bec99471c630
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289648"
---
# <a name="generating-proof-of-possession-tokens-for-rolling-keys"></a>Geração de tokens de prova de posse para chaves de rolagem

Você pode usar os métodos **addKey** e **RemoveKey** definidos no [aplicativo](/graph/resources/application?view=graph-rest-v1.0) e recursos do [servicePrincipalName](/graph/resources/serviceprincipal?view=graph-rest-v1.0) para acumular chaves de expiração programaticamente.

Como parte da solicitação de validação para esses métodos, uma prova de posse de uma chave existente é verificada para que os métodos possam ser chamados. A prova é representada por um token JWT auto-assinado. Esse token JWT deve ser assinado usando a chave privada de um dos certificados válidos existentes do aplicativo. O tempo de vida do token não deve exceder 10 minutos.

> **Observação:** Os aplicativos que não têm certificados válidos existentes (nenhum certificado foi adicionado ainda, ou todos os certificados expiraram) não poderão usar essa ação de serviço. Você pode usar a operação [Atualizar aplicativo](/graph/api/application-update?view=graph-rest-v1.0) para executar uma atualização.

O token deve conter as seguintes declarações:

- `aud`-A audiência precisa ser `00000002-0000-0000-c000-000000000000` .
- `iss`– O emissor precisa ser a __ID__ do aplicativo que está fazendo a chamada.
- `nbf`-Não antes da hora.
- `exp`– O tempo de expiração deve ser "NBF" + 10 minutos.

Você pode usar o exemplo de código a seguir para gerar esse token de prova de posse.

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
