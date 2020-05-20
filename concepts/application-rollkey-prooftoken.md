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
# <a name="generating-proof-of-possession-tokens-for-rolling-keys"></a><span data-ttu-id="a4f00-104">Geração de tokens de prova de posse para chaves de rolagem</span><span class="sxs-lookup"><span data-stu-id="a4f00-104">Generating proof of possession tokens for rolling keys</span></span>

<span data-ttu-id="a4f00-105">Você pode usar os métodos **addKey** e **RemoveKey** definidos no [aplicativo](/graph/resources/application?view=graph-rest-v1.0) e recursos do [servicePrincipalName](/graph/resources/serviceprincipal?view=graph-rest-v1.0) para acumular chaves de expiração programaticamente.</span><span class="sxs-lookup"><span data-stu-id="a4f00-105">You can use the **addKey** and **removeKey** methods defined on the [application](/graph/resources/application?view=graph-rest-v1.0) and [servicePrincipal](/graph/resources/serviceprincipal?view=graph-rest-v1.0) resources to roll expiring keys programmatically.</span></span>

<span data-ttu-id="a4f00-106">Como parte da solicitação de validação para esses métodos, uma prova de posse de uma chave existente é verificada para que os métodos possam ser chamados.</span><span class="sxs-lookup"><span data-stu-id="a4f00-106">As part of the request validation for these methods, a proof of possession of an existing key is verified before the methods can be invoked.</span></span> <span data-ttu-id="a4f00-107">A prova é representada por um token JWT auto-assinado.</span><span class="sxs-lookup"><span data-stu-id="a4f00-107">The proof is represented by a self-signed JWT token.</span></span> <span data-ttu-id="a4f00-108">Esse token JWT deve ser assinado usando a chave privada de um dos certificados válidos existentes do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a4f00-108">This JWT token must be signed using the private key of one of the application's existing valid certificates.</span></span> <span data-ttu-id="a4f00-109">O tempo de vida do token não deve exceder 10 minutos.</span><span class="sxs-lookup"><span data-stu-id="a4f00-109">The token lifespan should not exceed 10 minutes.</span></span>

> <span data-ttu-id="a4f00-110">**Observação:** Os aplicativos que não têm certificados válidos existentes (nenhum certificado foi adicionado ainda, ou todos os certificados expiraram) não poderão usar essa ação de serviço.</span><span class="sxs-lookup"><span data-stu-id="a4f00-110">**Note:** Applications that don’t have any existing valid certificates (no certificates have been added yet, or all certificates have expired), won’t be able to use this service action.</span></span> <span data-ttu-id="a4f00-111">Você pode usar a operação [Atualizar aplicativo](/graph/api/application-update?view=graph-rest-v1.0) para executar uma atualização.</span><span class="sxs-lookup"><span data-stu-id="a4f00-111">You can use the [Update application](/graph/api/application-update?view=graph-rest-v1.0) operation to perform an update instead.</span></span>

<span data-ttu-id="a4f00-112">O token deve conter as seguintes declarações:</span><span class="sxs-lookup"><span data-stu-id="a4f00-112">The token should contain the following claims:</span></span>

- <span data-ttu-id="a4f00-113">`aud`-A audiência precisa ser `00000002-0000-0000-c000-000000000000` .</span><span class="sxs-lookup"><span data-stu-id="a4f00-113">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span>
- <span data-ttu-id="a4f00-114">`iss`– O emissor precisa ser a __ID__ do aplicativo que está fazendo a chamada.</span><span class="sxs-lookup"><span data-stu-id="a4f00-114">`iss` - Issuer needs to be the __id__  of the application that is making the call.</span></span>
- <span data-ttu-id="a4f00-115">`nbf`-Não antes da hora.</span><span class="sxs-lookup"><span data-stu-id="a4f00-115">`nbf` - Not before time.</span></span>
- <span data-ttu-id="a4f00-116">`exp`– O tempo de expiração deve ser "NBF" + 10 minutos.</span><span class="sxs-lookup"><span data-stu-id="a4f00-116">`exp` - Expiration time should be "nbf" + 10 mins.</span></span>

<span data-ttu-id="a4f00-117">Você pode usar o exemplo de código a seguir para gerar esse token de prova de posse.</span><span class="sxs-lookup"><span data-stu-id="a4f00-117">You can use the following code example to generate this proof of possession token.</span></span>

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
