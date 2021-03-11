---
title: Tipo de recurso authenticationDetail
description: Fornece os detalhes de autenticação para uma login do usuário, como informações de autenticação multifatória (MFA) e detalhes PTA/PHS.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 134c3e502fa39fea626216315056adfeef5aef13
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720333"
---
# <a name="authenticationdetail-resource-type"></a><span data-ttu-id="a3ac2-103">Tipo de recurso authenticationDetail</span><span class="sxs-lookup"><span data-stu-id="a3ac2-103">authenticationDetail resource type</span></span>

<span data-ttu-id="a3ac2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3ac2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3ac2-105">Fornece os detalhes de autenticação para uma login do usuário, como informações de autenticação multifatória (MFA) e detalhes PTA/PHS.</span><span class="sxs-lookup"><span data-stu-id="a3ac2-105">Provides the authentication details for a user sign-in, such as multi-factor authentication (MFA) information and PTA/PHS details.</span></span>

## <a name="properties"></a><span data-ttu-id="a3ac2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a3ac2-106">Properties</span></span>

| <span data-ttu-id="a3ac2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3ac2-107">Property</span></span>                       | <span data-ttu-id="a3ac2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3ac2-108">Type</span></span>           | <span data-ttu-id="a3ac2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3ac2-109">Description</span></span>                                                                                                                                                                                                              |
|:-------------------------------|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a3ac2-110">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a3ac2-110">authenticationMethod</span></span>           | <span data-ttu-id="a3ac2-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3ac2-111">String</span></span>         | <span data-ttu-id="a3ac2-112">O tipo de método de autenticação usado para executar esta etapa de autenticação.</span><span class="sxs-lookup"><span data-stu-id="a3ac2-112">The type of authentication method used to perform this step of authentication.</span></span> <span data-ttu-id="a3ac2-113">Valores possíveis: `Password` , , , , , `SMS` `Voice` `Authenticator App` `Software OATH token` `Satisfied by token` .</span><span class="sxs-lookup"><span data-stu-id="a3ac2-113">Possible values: `Password`, `SMS`, `Voice`, `Authenticator App`, `Software OATH token`, `Satisfied by token`.</span></span>                            |
| <span data-ttu-id="a3ac2-114">authenticationMethodDetail</span><span class="sxs-lookup"><span data-stu-id="a3ac2-114">authenticationMethodDetail</span></span>     | <span data-ttu-id="a3ac2-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3ac2-115">String</span></span>         | <span data-ttu-id="a3ac2-116">Detalhes sobre o método de autenticação usado para executar essa etapa de autenticação.</span><span class="sxs-lookup"><span data-stu-id="a3ac2-116">Details about the authentication method used to perform this authentication step.</span></span> <span data-ttu-id="a3ac2-117">Por exemplo, número de telefone (para SMS e voz), nome do dispositivo (para aplicativo Autenticador) e fonte de senha (por exemplo, nuvem, AD FS, PTA, PHS).</span><span class="sxs-lookup"><span data-stu-id="a3ac2-117">For example, phone number (for SMS and voice), device name (for Authenticator app), and password source (e.g. cloud, AD FS, PTA, PHS).</span></span> |
| <span data-ttu-id="a3ac2-118">authenticationStepDateTime</span><span class="sxs-lookup"><span data-stu-id="a3ac2-118">authenticationStepDateTime</span></span>     | <span data-ttu-id="a3ac2-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3ac2-119">DateTimeOffset</span></span> | <span data-ttu-id="a3ac2-120">Representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a3ac2-120">Represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a3ac2-121">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="a3ac2-121">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>                                           |
| <span data-ttu-id="a3ac2-122">authenticationStepRequirement</span><span class="sxs-lookup"><span data-stu-id="a3ac2-122">authenticationStepRequirement</span></span>  | <span data-ttu-id="a3ac2-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3ac2-123">String</span></span>         | <span data-ttu-id="a3ac2-124">A etapa de autenticação que isso satisfez.</span><span class="sxs-lookup"><span data-stu-id="a3ac2-124">The step of authentication that this satisfied.</span></span> <span data-ttu-id="a3ac2-125">Por exemplo, autenticação primária ou autenticação multifa factor.</span><span class="sxs-lookup"><span data-stu-id="a3ac2-125">For example, primary authentication, or multi-factor authentication.</span></span>                                                                                                     |
| <span data-ttu-id="a3ac2-126">authenticationStepResultDetail</span><span class="sxs-lookup"><span data-stu-id="a3ac2-126">authenticationStepResultDetail</span></span> | <span data-ttu-id="a3ac2-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3ac2-127">String</span></span>         | <span data-ttu-id="a3ac2-128">Detalhes sobre por que a etapa foi bem-sucedida ou falhou.</span><span class="sxs-lookup"><span data-stu-id="a3ac2-128">Details about why the step succeeded or failed.</span></span> <span data-ttu-id="a3ac2-129">Por exemplo, o usuário é bloqueado, o código de fraude inserido, nenhuma entrada de telefone - tempo de tempo, telefone inacessível ou declaração em token.</span><span class="sxs-lookup"><span data-stu-id="a3ac2-129">For examples, user is blocked, fraud code entered, no phone input - timed out, phone unreachable, or claim in token.</span></span>                                                     |
| <span data-ttu-id="a3ac2-130">bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="a3ac2-130">succeeded</span></span>                      | <span data-ttu-id="a3ac2-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="a3ac2-131">Boolean</span></span>        | <span data-ttu-id="a3ac2-132">Indica o status da etapa de autenticação.</span><span class="sxs-lookup"><span data-stu-id="a3ac2-132">Indicates the status of the authentication step.</span></span> <span data-ttu-id="a3ac2-133">Valores possíveis: `succeeded` , `failed` .</span><span class="sxs-lookup"><span data-stu-id="a3ac2-133">Possible values: `succeeded`, `failed`.</span></span>                                                                                                                                 |

## <a name="json-representation"></a><span data-ttu-id="a3ac2-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a3ac2-134">JSON representation</span></span>

<span data-ttu-id="a3ac2-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a3ac2-135">The following is a JSON representation of the resource.</span></span>

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

