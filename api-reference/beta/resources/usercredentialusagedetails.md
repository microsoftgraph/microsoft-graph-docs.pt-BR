---
title: tipo de recurso userCredentialUsageDetails
description: Representa o uso de redefinição de senha de autoatendimento para um determinado locatário.
localization_priority: Normal
author: besiler
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 6ac0e1b8b73b019636e460772975da7a4f0505a1
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524236"
---
# <a name="usercredentialusagedetails-resource-type"></a><span data-ttu-id="c901d-103">tipo de recurso userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="c901d-103">userCredentialUsageDetails resource type</span></span>

<span data-ttu-id="c901d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c901d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c901d-105">Representa o uso de redefinição de senha de autoatendimento para um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="c901d-105">Represents the self-service password reset usage for a given tenant.</span></span> <span data-ttu-id="c901d-106">Os detalhes incluem informações do usuário, status da redefinição e o motivo da falha.</span><span class="sxs-lookup"><span data-stu-id="c901d-106">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="methods"></a><span data-ttu-id="c901d-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c901d-107">Methods</span></span>

| <span data-ttu-id="c901d-108">Método</span><span class="sxs-lookup"><span data-stu-id="c901d-108">Method</span></span>       | <span data-ttu-id="c901d-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c901d-109">Return Type</span></span> | <span data-ttu-id="c901d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c901d-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c901d-111">Listar userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="c901d-111">List userCredentialUsageDetails</span></span>](../api/reportroot-list-usercredentialusagedetails.md) | <span data-ttu-id="c901d-112">userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="c901d-112">userCredentialUsageDetails</span></span> | <span data-ttu-id="c901d-113">Ler propriedades e relações de um objeto userCredentialUsageDetails.</span><span class="sxs-lookup"><span data-stu-id="c901d-113">Read properties and relationships of a userCredentialUsageDetails object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c901d-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c901d-114">Properties</span></span>

| <span data-ttu-id="c901d-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c901d-115">Property</span></span>     | <span data-ttu-id="c901d-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="c901d-116">Type</span></span>        | <span data-ttu-id="c901d-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="c901d-117">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c901d-118">authMethod</span><span class="sxs-lookup"><span data-stu-id="c901d-118">authMethod</span></span> | <span data-ttu-id="c901d-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c901d-119">string</span></span> | <span data-ttu-id="c901d-120">Representa o método de autenticação usado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="c901d-120">Represents the authentication method that the user used.</span></span> <span data-ttu-id="c901d-121">Os valores possíveis são: `email` , `mobileSMS` ,, `mobileCall` `officePhone` , `securityQuestion` (usado somente para redefinição de senha de autoatendimento), e (somente para o `appNotification` `appCode` `alternateMobileCall` registro).</span><span class="sxs-lookup"><span data-stu-id="c901d-121">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobileCall` (supported only in registration).</span></span> |
| <span data-ttu-id="c901d-122">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="c901d-122">eventDateTime</span></span> | <span data-ttu-id="c901d-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c901d-123">DateTimeOffset</span></span> | <span data-ttu-id="c901d-124">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c901d-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c901d-125">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c901d-125">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
| <span data-ttu-id="c901d-126">failureReason</span><span class="sxs-lookup"><span data-stu-id="c901d-126">failureReason</span></span> | <span data-ttu-id="c901d-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c901d-127">String</span></span> | <span data-ttu-id="c901d-128">Fornece o motivo da falha para o fluxo de trabalho de redefinição ou registro correspondente.</span><span class="sxs-lookup"><span data-stu-id="c901d-128">Provides the failure reason for the corresponding reset or registration workflow.</span></span> |
| <span data-ttu-id="c901d-129">apresentam</span><span class="sxs-lookup"><span data-stu-id="c901d-129">feature</span></span> | <span data-ttu-id="c901d-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c901d-130">string</span></span> | <span data-ttu-id="c901d-131">Os valores possíveis são: `registration` e `reset` .</span><span class="sxs-lookup"><span data-stu-id="c901d-131">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="c901d-132">id</span><span class="sxs-lookup"><span data-stu-id="c901d-132">id</span></span> | <span data-ttu-id="c901d-133">String</span><span class="sxs-lookup"><span data-stu-id="c901d-133">String</span></span> | <span data-ttu-id="c901d-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c901d-134">Read-only.</span></span> <span data-ttu-id="c901d-135">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="c901d-135">The unique identifier for the activity.</span></span> <span data-ttu-id="c901d-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c901d-136">Read-only.</span></span>|
| <span data-ttu-id="c901d-137">IsSuccess</span><span class="sxs-lookup"><span data-stu-id="c901d-137">isSuccess</span></span> | <span data-ttu-id="c901d-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="c901d-138">Boolean</span></span> | <span data-ttu-id="c901d-139">Indica êxito ou falha do fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c901d-139">Indicates success or failure of the workflow.</span></span> |
| <span data-ttu-id="c901d-140">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c901d-140">userDisplayName</span></span> | <span data-ttu-id="c901d-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c901d-141">String</span></span> | <span data-ttu-id="c901d-142">Nome de usuário do usuário que está executando o fluxo de trabalho de redefinição ou registro.</span><span class="sxs-lookup"><span data-stu-id="c901d-142">User name of the user performing the reset or registration workflow.</span></span> |
| <span data-ttu-id="c901d-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c901d-143">userPrincipalName</span></span> | <span data-ttu-id="c901d-144">String</span><span class="sxs-lookup"><span data-stu-id="c901d-144">String</span></span> | <span data-ttu-id="c901d-145">Nome principal do usuário que está executando o fluxo de trabalho de redefinição ou registro.</span><span class="sxs-lookup"><span data-stu-id="c901d-145">User principal name of the user performing the reset or registration workflow.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c901d-146">Relações</span><span class="sxs-lookup"><span data-stu-id="c901d-146">Relationships</span></span>

<span data-ttu-id="c901d-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c901d-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c901d-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c901d-148">JSON representation</span></span>

<span data-ttu-id="c901d-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c901d-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "feature":"string",
  "userPrincipalName":"String",
  "userDisplayName": "String",
  "isSuccess" : true,
  "authMethod": "string",
  "failureReason": "String",
  "eventDateTime" : "DateTimeOffset"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userCredentialUsageDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

