---
title: tipo de recurso authenticationDetail
description: Fornece os detalhes de autenticação para uma entrada de usuário, como informações de autenticação multifator (MFA) e detalhes de PTA/PHS.
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 14f2121aabaae591187d3033903e569b482b8727
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521240"
---
# <a name="authenticationdetail-resource-type"></a><span data-ttu-id="f1421-103">tipo de recurso authenticationDetail</span><span class="sxs-lookup"><span data-stu-id="f1421-103">authenticationDetail resource type</span></span>

<span data-ttu-id="f1421-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1421-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1421-105">Fornece os detalhes de autenticação para uma entrada de usuário, como informações de autenticação multifator (MFA) e detalhes de PTA/PHS.</span><span class="sxs-lookup"><span data-stu-id="f1421-105">Provides the authentication details for a user sign-in, such as multi-factor authentication (MFA) information and PTA/PHS details.</span></span>

## <a name="properties"></a><span data-ttu-id="f1421-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1421-106">Properties</span></span>

| <span data-ttu-id="f1421-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1421-107">Property</span></span>                       | <span data-ttu-id="f1421-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1421-108">Type</span></span>           | <span data-ttu-id="f1421-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1421-109">Description</span></span>                                                                                                                                                                                                              |
|:-------------------------------|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f1421-110">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f1421-110">authenticationMethod</span></span>           | <span data-ttu-id="f1421-111">String</span><span class="sxs-lookup"><span data-stu-id="f1421-111">String</span></span>         | <span data-ttu-id="f1421-112">O tipo de método de autenticação usado para executar esta etapa de autenticação.</span><span class="sxs-lookup"><span data-stu-id="f1421-112">The type of authentication method used to perform this step of authentication.</span></span> <span data-ttu-id="f1421-113">Valores possíveis: `Password` , `SMS` ,,, `Voice` `Authenticator App` `Software OATH token` , `Satisfied by token` .</span><span class="sxs-lookup"><span data-stu-id="f1421-113">Possible values: `Password`, `SMS`, `Voice`, `Authenticator App`, `Software OATH token`, `Satisfied by token`.</span></span>                            |
| <span data-ttu-id="f1421-114">authenticationMethodDetail</span><span class="sxs-lookup"><span data-stu-id="f1421-114">authenticationMethodDetail</span></span>     | <span data-ttu-id="f1421-115">String</span><span class="sxs-lookup"><span data-stu-id="f1421-115">String</span></span>         | <span data-ttu-id="f1421-116">Detalhes sobre o método de autenticação usado para executar esta etapa de autenticação.</span><span class="sxs-lookup"><span data-stu-id="f1421-116">Details about the authentication method used to perform this authentication step.</span></span> <span data-ttu-id="f1421-117">Por exemplo, número de telefone (para SMS e voz), nome do dispositivo (para o aplicativo autenticador) e a fonte da senha (por exemplo, nuvem, AD FS, PTA, PHS).</span><span class="sxs-lookup"><span data-stu-id="f1421-117">For example, phone number (for SMS and voice), device name (for Authenticator app), and password source (e.g. cloud, AD FS, PTA, PHS).</span></span> |
| <span data-ttu-id="f1421-118">authenticationStepDateTime</span><span class="sxs-lookup"><span data-stu-id="f1421-118">authenticationStepDateTime</span></span>     | <span data-ttu-id="f1421-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1421-119">DateTimeOffset</span></span> | <span data-ttu-id="f1421-120">Representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f1421-120">Represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f1421-121">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f1421-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>                                           |
| <span data-ttu-id="f1421-122">authenticationStepRequirement</span><span class="sxs-lookup"><span data-stu-id="f1421-122">authenticationStepRequirement</span></span>  | <span data-ttu-id="f1421-123">String</span><span class="sxs-lookup"><span data-stu-id="f1421-123">String</span></span>         | <span data-ttu-id="f1421-124">A etapa de autenticação atendida.</span><span class="sxs-lookup"><span data-stu-id="f1421-124">The step of authentication that this satisfied.</span></span> <span data-ttu-id="f1421-125">Por exemplo, autenticação primária ou autenticação multifator.</span><span class="sxs-lookup"><span data-stu-id="f1421-125">For example, primary authentication, or multi-factor authentication.</span></span>                                                                                                     |
| <span data-ttu-id="f1421-126">authenticationStepResultDetail</span><span class="sxs-lookup"><span data-stu-id="f1421-126">authenticationStepResultDetail</span></span> | <span data-ttu-id="f1421-127">String</span><span class="sxs-lookup"><span data-stu-id="f1421-127">String</span></span>         | <span data-ttu-id="f1421-128">Detalhes sobre por que a etapa foi bem-sucedida ou falhou.</span><span class="sxs-lookup"><span data-stu-id="f1421-128">Details about why the step succeeded or failed.</span></span> <span data-ttu-id="f1421-129">Por exemplo, o usuário é bloqueado, o código de fraude inserido, nenhuma entrada de telefone-tempo limite, telefone inacessível ou declaração no token.</span><span class="sxs-lookup"><span data-stu-id="f1421-129">For examples, user is blocked, fraud code entered, no phone input - timed out, phone unreachable, or claim in token.</span></span>                                                     |
| <span data-ttu-id="f1421-130">adicionada</span><span class="sxs-lookup"><span data-stu-id="f1421-130">succeeded</span></span>                      | <span data-ttu-id="f1421-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1421-131">Boolean</span></span>        | <span data-ttu-id="f1421-132">Indica o status da etapa de autenticação.</span><span class="sxs-lookup"><span data-stu-id="f1421-132">Indicates the status of the authentication step.</span></span> <span data-ttu-id="f1421-133">Valores possíveis: `succeeded` , `failed` .</span><span class="sxs-lookup"><span data-stu-id="f1421-133">Possible values: `succeeded`, `failed`.</span></span>                                                                                                                                 |

## <a name="json-representation"></a><span data-ttu-id="f1421-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1421-134">JSON representation</span></span>

<span data-ttu-id="f1421-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1421-135">The following is a JSON representation of the resource.</span></span>

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

