---
title: Gerando um token de comprovação de posse para sobrepor chaves
description: Como parte da validação da solicitação para os métodos addKey e removeKey, é necessário um token de comprovação de posse. Este documento fornece orientação para gerar o token de comprovação de posse.
localization_priority: Priority
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: b0e0384ab440bb08eb3b708c4ad057da42986c5c
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330089"
---
# <a name="generating-proof-of-possession-tokens-for-rolling-keys"></a><span data-ttu-id="cbf14-104">Gerando um token de comprovação de posse para sobrepor chaves</span><span class="sxs-lookup"><span data-stu-id="cbf14-104">Generating proof of possession tokens for rolling keys</span></span>

<span data-ttu-id="cbf14-105">Você pode usar os métodos **addKey** e **removeKey** definidos no [aplicativo](/graph/api/resources/application?view=graph-rest-1.0) e recursos [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) para acumular as chaves expiradas por programação.</span><span class="sxs-lookup"><span data-stu-id="cbf14-105">You can use the **addKey** and **removeKey** methods defined on the [application](/graph/api/resources/application?view=graph-rest-1.0) and [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) resources to roll expiring keys programmatically.</span></span>

<span data-ttu-id="cbf14-106">Como parte da solicitação de validação para esses métodos, uma comprovação de posse de uma chave existente é verificada antes que os métodos possam ser invocados.</span><span class="sxs-lookup"><span data-stu-id="cbf14-106">As part of the request validation for these methods, a proof of possession of an existing key is verified before the methods can be invoked.</span></span> <span data-ttu-id="cbf14-107">As comprovações são representadas por um token JWT autoassinado.</span><span class="sxs-lookup"><span data-stu-id="cbf14-107">The proof is represented by a self-signed JWT token.</span></span> <span data-ttu-id="cbf14-108">Esse token de JWT deve ser assinado usando a chave privada de um dos certificados válidos existentes do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cbf14-108">This JWT token must be signed using the private key of one of the application's existing valid certificates.</span></span> <span data-ttu-id="cbf14-109">O tempo de vida do token não deve exceder 10 minutos.</span><span class="sxs-lookup"><span data-stu-id="cbf14-109">The token lifespan should not exceed 10 minutes.</span></span>

> <span data-ttu-id="cbf14-110">**Observação:** Aplicativos que não têm certificados válidos existentes (nenhum certificado foi adicionado ainda, ou todos os certificados expiraram), não poderão usar essa ação de serviço.</span><span class="sxs-lookup"><span data-stu-id="cbf14-110">**Note:** Applications that don’t have any existing valid certificates (no certificates have been added yet, or all certificates have expired), won’t be able to use this service action.</span></span> <span data-ttu-id="cbf14-111">Você pode usar a operação [Atualizar aplicativo](/graph/api/application-update?view=graph-rest-v1.0) para executar uma atualização.</span><span class="sxs-lookup"><span data-stu-id="cbf14-111">You can use the [Update application](/graph/api/application-update?view=graph-rest-v1.0) operation to perform an update instead.</span></span>

<span data-ttu-id="cbf14-112">O token deve conter os seguintes argumentos:</span><span class="sxs-lookup"><span data-stu-id="cbf14-112">The token should contain the following claims:</span></span>

- <span data-ttu-id="cbf14-113">`aud` – A audiência deve ser `00000002-0000-0000-c000-000000000000`.</span><span class="sxs-lookup"><span data-stu-id="cbf14-113">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span>
- <span data-ttu-id="cbf14-114">`iss` - O emissor deve ser o __ID__ do aplicativo que está fazendo a chamada.</span><span class="sxs-lookup"><span data-stu-id="cbf14-114">`iss` - Issuer needs to be the __id__  of the application that is making the call.</span></span>
- <span data-ttu-id="cbf14-115">`nbf` – Não antes da hora.</span><span class="sxs-lookup"><span data-stu-id="cbf14-115">`nbf` - Not before time.</span></span>
- <span data-ttu-id="cbf14-116">`exp` – O tempo de expiração deve ser "nbf" + 10 min.</span><span class="sxs-lookup"><span data-stu-id="cbf14-116">`exp` - Expiration time should be "nbf" + 10 mins.</span></span>

<span data-ttu-id="cbf14-117">Você pode usar o seguinte exemplo de código para gerar esse token de comprovação de posse.</span><span class="sxs-lookup"><span data-stu-id="cbf14-117">You can use the following code example to generate this proof of possession token.</span></span>

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
