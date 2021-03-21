---
title: Tipo de recurso authenticationDetail
description: Fornece os detalhes de autenticação para uma login do usuário, como informações de autenticação multifatória (MFA) e detalhes PTA/PHS.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 0f7042b8b2be369c97e19cb038d7cf82fe07e96d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964554"
---
# <a name="authenticationdetail-resource-type"></a><span data-ttu-id="34528-103">Tipo de recurso authenticationDetail</span><span class="sxs-lookup"><span data-stu-id="34528-103">authenticationDetail resource type</span></span>

<span data-ttu-id="34528-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34528-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34528-105">Fornece os detalhes de autenticação para uma login do usuário, como informações de autenticação multifatória (MFA) e detalhes PTA/PHS.</span><span class="sxs-lookup"><span data-stu-id="34528-105">Provides the authentication details for a user sign-in, such as multi-factor authentication (MFA) information and PTA/PHS details.</span></span>

## <a name="properties"></a><span data-ttu-id="34528-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34528-106">Properties</span></span>

| <span data-ttu-id="34528-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34528-107">Property</span></span>                       | <span data-ttu-id="34528-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="34528-108">Type</span></span>           | <span data-ttu-id="34528-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="34528-109">Description</span></span>                                                                                                                                                                                                              |
|:-------------------------------|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="34528-110">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="34528-110">authenticationMethod</span></span>           | <span data-ttu-id="34528-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34528-111">String</span></span>         | <span data-ttu-id="34528-112">O tipo de método de autenticação usado para executar esta etapa de autenticação.</span><span class="sxs-lookup"><span data-stu-id="34528-112">The type of authentication method used to perform this step of authentication.</span></span> <span data-ttu-id="34528-113">Valores possíveis: `Password` , , , , , , `SMS` `Voice` `Authenticator App` `Software OATH token` `Satisfied by token` `Previously satisfied` .</span><span class="sxs-lookup"><span data-stu-id="34528-113">Possible values: `Password`, `SMS`, `Voice`, `Authenticator App`, `Software OATH token`, `Satisfied by token`, `Previously satisfied`.</span></span>                            |
| <span data-ttu-id="34528-114">authenticationMethodDetail</span><span class="sxs-lookup"><span data-stu-id="34528-114">authenticationMethodDetail</span></span>     | <span data-ttu-id="34528-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34528-115">String</span></span>         | <span data-ttu-id="34528-116">Detalhes sobre o método de autenticação usado para executar essa etapa de autenticação.</span><span class="sxs-lookup"><span data-stu-id="34528-116">Details about the authentication method used to perform this authentication step.</span></span> <span data-ttu-id="34528-117">Por exemplo, número de telefone (para SMS e voz), nome do dispositivo (para aplicativo Autenticador) e fonte de senha (por exemplo, nuvem, AD FS, PTA, PHS).</span><span class="sxs-lookup"><span data-stu-id="34528-117">For example, phone number (for SMS and voice), device name (for Authenticator app), and password source (e.g. cloud, AD FS, PTA, PHS).</span></span> |
| <span data-ttu-id="34528-118">authenticationStepDateTime</span><span class="sxs-lookup"><span data-stu-id="34528-118">authenticationStepDateTime</span></span>     | <span data-ttu-id="34528-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34528-119">DateTimeOffset</span></span> | <span data-ttu-id="34528-120">Representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="34528-120">Represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="34528-121">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="34528-121">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>                                           |
| <span data-ttu-id="34528-122">authenticationStepRequirement</span><span class="sxs-lookup"><span data-stu-id="34528-122">authenticationStepRequirement</span></span>  | <span data-ttu-id="34528-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34528-123">String</span></span>         | <span data-ttu-id="34528-124">A etapa de autenticação que isso satisfez.</span><span class="sxs-lookup"><span data-stu-id="34528-124">The step of authentication that this satisfied.</span></span> <span data-ttu-id="34528-125">Por exemplo, autenticação primária ou autenticação multifa factor.</span><span class="sxs-lookup"><span data-stu-id="34528-125">For example, primary authentication, or multi-factor authentication.</span></span>                                                                                                     |
| <span data-ttu-id="34528-126">authenticationStepResultDetail</span><span class="sxs-lookup"><span data-stu-id="34528-126">authenticationStepResultDetail</span></span> | <span data-ttu-id="34528-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34528-127">String</span></span>         | <span data-ttu-id="34528-128">Detalhes sobre por que a etapa foi bem-sucedida ou falhou.</span><span class="sxs-lookup"><span data-stu-id="34528-128">Details about why the step succeeded or failed.</span></span> <span data-ttu-id="34528-129">Por exemplo, o usuário é bloqueado, o código de fraude inserido, nenhuma entrada de telefone - tempo de tempo, telefone inacessível ou declaração em token.</span><span class="sxs-lookup"><span data-stu-id="34528-129">For examples, user is blocked, fraud code entered, no phone input - timed out, phone unreachable, or claim in token.</span></span>                                                     |
| <span data-ttu-id="34528-130">bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="34528-130">succeeded</span></span>                      | <span data-ttu-id="34528-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="34528-131">Boolean</span></span>        | <span data-ttu-id="34528-132">Indica o status da etapa de autenticação.</span><span class="sxs-lookup"><span data-stu-id="34528-132">Indicates the status of the authentication step.</span></span> <span data-ttu-id="34528-133">Valores possíveis: `succeeded` , `failed` .</span><span class="sxs-lookup"><span data-stu-id="34528-133">Possible values: `succeeded`, `failed`.</span></span>                                                                                                                                 |

## <a name="json-representation"></a><span data-ttu-id="34528-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34528-134">JSON representation</span></span>

<span data-ttu-id="34528-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34528-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authenticationDetail",
  "baseType": null
}-->

```json
{
  "authenticationMethod": "String",
  "authenticationMethodDetail": "String",
  "authenticationStepDateTime": "String (timestamp)",
  "authenticationStepRequirement": "String",
  "authenticationStepResultDetail": "String",
  "succeeded": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "authenticationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

