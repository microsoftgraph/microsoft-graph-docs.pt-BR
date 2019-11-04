---
title: tipo de recurso authenticationDetail
description: Fornece os detalhes de autenticação para uma entrada de usuário, como informações de autenticação multifator (MFA) e detalhes de PTA/PHS.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 715685ee485b538d6be3dd45cb87949483324382
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939394"
---
# <a name="authenticationdetail-resource-type"></a><span data-ttu-id="3fd77-103">tipo de recurso authenticationDetail</span><span class="sxs-lookup"><span data-stu-id="3fd77-103">authenticationDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fd77-104">Fornece os detalhes de autenticação para uma entrada de usuário, como informações de autenticação multifator (MFA) e detalhes de PTA/PHS.</span><span class="sxs-lookup"><span data-stu-id="3fd77-104">Provides the authentication details for a user sign-in, such as multi-factor authentication (MFA) information and PTA/PHS details.</span></span>

## <a name="properties"></a><span data-ttu-id="3fd77-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3fd77-105">Properties</span></span>

| <span data-ttu-id="3fd77-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3fd77-106">Property</span></span>     | <span data-ttu-id="3fd77-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fd77-107">Type</span></span>        | <span data-ttu-id="3fd77-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fd77-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3fd77-109">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3fd77-109">authenticationMethod</span></span>|<span data-ttu-id="3fd77-110">String</span><span class="sxs-lookup"><span data-stu-id="3fd77-110">String</span></span>||<span data-ttu-id="3fd77-111">O tipo de método de autenticação usado para executar esta etapa de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3fd77-111">The type of authentication method used to perform this step of authentication.</span></span> <span data-ttu-id="3fd77-112">Valores possíveis: `Password`, `SMS`, `Voice`` Authenticator App`,, `Software OATH token`, `Satisfied by token`.</span><span class="sxs-lookup"><span data-stu-id="3fd77-112">Possible values: `Password`, `SMS`, `Voice`,` Authenticator App`, `Software OATH token`, `Satisfied by token`.</span></span>|
|<span data-ttu-id="3fd77-113">authenticationMethodDetail</span><span class="sxs-lookup"><span data-stu-id="3fd77-113">authenticationMethodDetail</span></span>|<span data-ttu-id="3fd77-114">String</span><span class="sxs-lookup"><span data-stu-id="3fd77-114">String</span></span>|<span data-ttu-id="3fd77-115">Detalhes sobre o método de autenticação usado para executar esta etapa de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3fd77-115">Details about the authentication method used to perform this authentication step.</span></span> <span data-ttu-id="3fd77-116">Por exemplo, número de telefone (para SMS e voz), nome do dispositivo (para o aplicativo autenticador) e a fonte da senha (por exemplo, nuvem, AD FS, PTA, PHS).</span><span class="sxs-lookup"><span data-stu-id="3fd77-116">For example, phone number (for SMS and voice), device name (for Authenticator app), and password source (e.g. cloud, AD FS, PTA, PHS).</span></span> |
|<span data-ttu-id="3fd77-117">authenticationStepDateTime</span><span class="sxs-lookup"><span data-stu-id="3fd77-117">authenticationStepDateTime</span></span>|<span data-ttu-id="3fd77-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fd77-118">DateTimeOffset</span></span>|<span data-ttu-id="3fd77-119">Representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3fd77-119">Represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3fd77-120">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3fd77-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
|<span data-ttu-id="3fd77-121">authenticationStepRequirement</span><span class="sxs-lookup"><span data-stu-id="3fd77-121">authenticationStepRequirement</span></span>|<span data-ttu-id="3fd77-122">String</span><span class="sxs-lookup"><span data-stu-id="3fd77-122">String</span></span>|<span data-ttu-id="3fd77-123">A etapa de autenticação atendida.</span><span class="sxs-lookup"><span data-stu-id="3fd77-123">The step of authentication that this satisfied.</span></span> <span data-ttu-id="3fd77-124">Por exemplo, autenticação primária ou autenticação multifator.</span><span class="sxs-lookup"><span data-stu-id="3fd77-124">For example, primary authentication, or multi-factor authentication.</span></span>|
|<span data-ttu-id="3fd77-125">authenticationStepResultDetail</span><span class="sxs-lookup"><span data-stu-id="3fd77-125">authenticationStepResultDetail</span></span>|<span data-ttu-id="3fd77-126">String</span><span class="sxs-lookup"><span data-stu-id="3fd77-126">String</span></span>|<span data-ttu-id="3fd77-127">Detalhes sobre por que a etapa foi bem-sucedida ou falhou.</span><span class="sxs-lookup"><span data-stu-id="3fd77-127">Details about why the step succeeded or failed.</span></span> <span data-ttu-id="3fd77-128">Por exemplo, o usuário é bloqueado, o código de fraude inserido, nenhuma entrada de telefone-tempo limite, telefone inacessível ou declaração no token.</span><span class="sxs-lookup"><span data-stu-id="3fd77-128">For examples, user is blocked, fraud code entered, no phone input - timed out, phone unreachable, or claim in token.</span></span>|
|<span data-ttu-id="3fd77-129">adicionada</span><span class="sxs-lookup"><span data-stu-id="3fd77-129">succeeded</span></span>|<span data-ttu-id="3fd77-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fd77-130">Boolean</span></span>|<span data-ttu-id="3fd77-131">Indica o status da etapa de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3fd77-131">Indicates the status of the authentication step.</span></span>|<span data-ttu-id="3fd77-132">Valores possíveis: `succeeded`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="3fd77-132">Possible values: `succeeded`, `failed`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3fd77-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3fd77-133">JSON representation</span></span>

<span data-ttu-id="3fd77-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3fd77-134">The following is a JSON representation of the resource.</span></span>

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