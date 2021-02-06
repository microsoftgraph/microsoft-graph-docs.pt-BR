---
title: Tipo de recurso authenticationDetail
description: Fornece os detalhes de autenticação para uma login do usuário, como informações de autenticação multifatória (MFA) e detalhes de PTA/PHS.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: b888ec232a95c821ab00f6baa16e787cfbc7dd7f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136623"
---
# <a name="authenticationdetail-resource-type"></a><span data-ttu-id="c2b28-103">Tipo de recurso authenticationDetail</span><span class="sxs-lookup"><span data-stu-id="c2b28-103">authenticationDetail resource type</span></span>

<span data-ttu-id="c2b28-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2b28-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2b28-105">Fornece os detalhes de autenticação para uma login do usuário, como informações de autenticação multifa factor (MFA) e detalhes de PTA/PHS.</span><span class="sxs-lookup"><span data-stu-id="c2b28-105">Provides the authentication details for a user sign-in, such as multi-factor authentication (MFA) information and PTA/PHS details.</span></span>

## <a name="properties"></a><span data-ttu-id="c2b28-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c2b28-106">Properties</span></span>

| <span data-ttu-id="c2b28-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2b28-107">Property</span></span>                       | <span data-ttu-id="c2b28-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2b28-108">Type</span></span>           | <span data-ttu-id="c2b28-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2b28-109">Description</span></span>                                                                                                                                                                                                              |
|:-------------------------------|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c2b28-110">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c2b28-110">authenticationMethod</span></span>           | <span data-ttu-id="c2b28-111">String</span><span class="sxs-lookup"><span data-stu-id="c2b28-111">String</span></span>         | <span data-ttu-id="c2b28-112">O tipo de método de autenticação usado para executar essa etapa de autenticação.</span><span class="sxs-lookup"><span data-stu-id="c2b28-112">The type of authentication method used to perform this step of authentication.</span></span> <span data-ttu-id="c2b28-113">Valores possíveis: `Password` , , , , `SMS` `Voice` `Authenticator App` `Software OATH token` `Satisfied by token` .</span><span class="sxs-lookup"><span data-stu-id="c2b28-113">Possible values: `Password`, `SMS`, `Voice`, `Authenticator App`, `Software OATH token`, `Satisfied by token`.</span></span>                            |
| <span data-ttu-id="c2b28-114">authenticationMethodDetail</span><span class="sxs-lookup"><span data-stu-id="c2b28-114">authenticationMethodDetail</span></span>     | <span data-ttu-id="c2b28-115">String</span><span class="sxs-lookup"><span data-stu-id="c2b28-115">String</span></span>         | <span data-ttu-id="c2b28-116">Detalhes sobre o método de autenticação usado para executar essa etapa de autenticação.</span><span class="sxs-lookup"><span data-stu-id="c2b28-116">Details about the authentication method used to perform this authentication step.</span></span> <span data-ttu-id="c2b28-117">Por exemplo, número de telefone (para SMS e voz), nome do dispositivo (para aplicativo Autenticador) e fonte de senha (por exemplo, nuvem, AD FS, PTA, PHS).</span><span class="sxs-lookup"><span data-stu-id="c2b28-117">For example, phone number (for SMS and voice), device name (for Authenticator app), and password source (e.g. cloud, AD FS, PTA, PHS).</span></span> |
| <span data-ttu-id="c2b28-118">authenticationStepDateTime</span><span class="sxs-lookup"><span data-stu-id="c2b28-118">authenticationStepDateTime</span></span>     | <span data-ttu-id="c2b28-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2b28-119">DateTimeOffset</span></span> | <span data-ttu-id="c2b28-120">Representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c2b28-120">Represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c2b28-121">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c2b28-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>                                           |
| <span data-ttu-id="c2b28-122">authenticationStepRequirement</span><span class="sxs-lookup"><span data-stu-id="c2b28-122">authenticationStepRequirement</span></span>  | <span data-ttu-id="c2b28-123">String</span><span class="sxs-lookup"><span data-stu-id="c2b28-123">String</span></span>         | <span data-ttu-id="c2b28-124">A etapa de autenticação que isso atendia.</span><span class="sxs-lookup"><span data-stu-id="c2b28-124">The step of authentication that this satisfied.</span></span> <span data-ttu-id="c2b28-125">Por exemplo, autenticação principal ou autenticação multifa factor.</span><span class="sxs-lookup"><span data-stu-id="c2b28-125">For example, primary authentication, or multi-factor authentication.</span></span>                                                                                                     |
| <span data-ttu-id="c2b28-126">authenticationStepResultDetail</span><span class="sxs-lookup"><span data-stu-id="c2b28-126">authenticationStepResultDetail</span></span> | <span data-ttu-id="c2b28-127">String</span><span class="sxs-lookup"><span data-stu-id="c2b28-127">String</span></span>         | <span data-ttu-id="c2b28-128">Detalhes sobre por que a etapa foi bem-sucedida ou falhou.</span><span class="sxs-lookup"><span data-stu-id="c2b28-128">Details about why the step succeeded or failed.</span></span> <span data-ttu-id="c2b28-129">Por exemplo, o usuário está bloqueado, o código de fraude inserido, nenhuma entrada de telefone - tempo exemplado, telefone inacessível ou declaração em token.</span><span class="sxs-lookup"><span data-stu-id="c2b28-129">For examples, user is blocked, fraud code entered, no phone input - timed out, phone unreachable, or claim in token.</span></span>                                                     |
| <span data-ttu-id="c2b28-130">succeeded</span><span class="sxs-lookup"><span data-stu-id="c2b28-130">succeeded</span></span>                      | <span data-ttu-id="c2b28-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2b28-131">Boolean</span></span>        | <span data-ttu-id="c2b28-132">Indica o status da etapa de autenticação.</span><span class="sxs-lookup"><span data-stu-id="c2b28-132">Indicates the status of the authentication step.</span></span> <span data-ttu-id="c2b28-133">Valores possíveis: `succeeded` , `failed` .</span><span class="sxs-lookup"><span data-stu-id="c2b28-133">Possible values: `succeeded`, `failed`.</span></span>                                                                                                                                 |

## <a name="json-representation"></a><span data-ttu-id="c2b28-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c2b28-134">JSON representation</span></span>

<span data-ttu-id="c2b28-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c2b28-135">The following is a JSON representation of the resource.</span></span>

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

