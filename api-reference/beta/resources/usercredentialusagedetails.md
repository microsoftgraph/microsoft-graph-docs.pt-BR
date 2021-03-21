---
title: Tipo de recurso userCredentialUsageDetails
description: Representa o uso de redefinição de senha de autoatendados para um determinado locatário.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: deb5c93570a9921bc1830bfcb0772d643eed68b7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958655"
---
# <a name="usercredentialusagedetails-resource-type"></a><span data-ttu-id="bb300-103">Tipo de recurso userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="bb300-103">userCredentialUsageDetails resource type</span></span>

<span data-ttu-id="bb300-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb300-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb300-105">Representa o uso de redefinição de senha de autoatendados para um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="bb300-105">Represents the self-service password reset usage for a given tenant.</span></span> <span data-ttu-id="bb300-106">Os detalhes incluem informações do usuário, status da redefinição e o motivo da falha.</span><span class="sxs-lookup"><span data-stu-id="bb300-106">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="methods"></a><span data-ttu-id="bb300-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="bb300-107">Methods</span></span>

| <span data-ttu-id="bb300-108">Método</span><span class="sxs-lookup"><span data-stu-id="bb300-108">Method</span></span>       | <span data-ttu-id="bb300-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bb300-109">Return Type</span></span> | <span data-ttu-id="bb300-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb300-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bb300-111">Listar userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="bb300-111">List userCredentialUsageDetails</span></span>](../api/reportroot-list-usercredentialusagedetails.md) | <span data-ttu-id="bb300-112">userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="bb300-112">userCredentialUsageDetails</span></span> | <span data-ttu-id="bb300-113">Ler propriedades e relações de um objeto userCredentialUsageDetails.</span><span class="sxs-lookup"><span data-stu-id="bb300-113">Read properties and relationships of a userCredentialUsageDetails object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bb300-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb300-114">Properties</span></span>

| <span data-ttu-id="bb300-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb300-115">Property</span></span>     | <span data-ttu-id="bb300-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb300-116">Type</span></span>        | <span data-ttu-id="bb300-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb300-117">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bb300-118">authMethod</span><span class="sxs-lookup"><span data-stu-id="bb300-118">authMethod</span></span> | <span data-ttu-id="bb300-119">usageAuthMethod</span><span class="sxs-lookup"><span data-stu-id="bb300-119">usageAuthMethod</span></span> | <span data-ttu-id="bb300-120">Representa o método de autenticação que o usuário usou.</span><span class="sxs-lookup"><span data-stu-id="bb300-120">Represents the authentication method that the user used.</span></span> <span data-ttu-id="bb300-121">Os valores possíveis são: , , , , , (usado apenas para redefinição de senha de `email` `mobileSMS` `mobileCall` `officePhone` `securityQuestion` autoatendido), `appNotification` , , , `appCode` `alternateMobileCall` (suportado somente no registro), `fido` , , `appPassword` ,`unknownFutureValue`</span><span class="sxs-lookup"><span data-stu-id="bb300-121">Possible values are:`email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, `alternateMobileCall` (supported only in registration), `fido`, `appPassword`,`unknownFutureValue`</span></span> |
| <span data-ttu-id="bb300-122">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="bb300-122">eventDateTime</span></span> | <span data-ttu-id="bb300-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb300-123">DateTimeOffset</span></span> | <span data-ttu-id="bb300-124">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="bb300-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bb300-125">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="bb300-125">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="bb300-126">failureReason</span><span class="sxs-lookup"><span data-stu-id="bb300-126">failureReason</span></span> | <span data-ttu-id="bb300-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb300-127">String</span></span> | <span data-ttu-id="bb300-128">Fornece o motivo da falha para o fluxo de trabalho de redefinição ou registro correspondente.</span><span class="sxs-lookup"><span data-stu-id="bb300-128">Provides the failure reason for the corresponding reset or registration workflow.</span></span> |
| <span data-ttu-id="bb300-129">feature</span><span class="sxs-lookup"><span data-stu-id="bb300-129">feature</span></span> | <span data-ttu-id="bb300-130">featureType</span><span class="sxs-lookup"><span data-stu-id="bb300-130">featureType</span></span> | <span data-ttu-id="bb300-131">Os valores possíveis são: `registration`, `reset`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="bb300-131">Possible values are: `registration`, `reset`, `unknownFutureValue`.</span></span> |
| <span data-ttu-id="bb300-132">id</span><span class="sxs-lookup"><span data-stu-id="bb300-132">id</span></span> | <span data-ttu-id="bb300-133">String</span><span class="sxs-lookup"><span data-stu-id="bb300-133">String</span></span> | <span data-ttu-id="bb300-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb300-134">Read-only.</span></span> <span data-ttu-id="bb300-135">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="bb300-135">The unique identifier for the activity.</span></span> <span data-ttu-id="bb300-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb300-136">Read-only.</span></span>|
| <span data-ttu-id="bb300-137">isSuccess</span><span class="sxs-lookup"><span data-stu-id="bb300-137">isSuccess</span></span> | <span data-ttu-id="bb300-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb300-138">Boolean</span></span> | <span data-ttu-id="bb300-139">Indica sucesso ou falha do fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="bb300-139">Indicates success or failure of the workflow.</span></span> |
| <span data-ttu-id="bb300-140">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="bb300-140">userDisplayName</span></span> | <span data-ttu-id="bb300-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb300-141">String</span></span> | <span data-ttu-id="bb300-142">Nome de usuário do usuário que executa o fluxo de trabalho de redefinição ou registro.</span><span class="sxs-lookup"><span data-stu-id="bb300-142">User name of the user performing the reset or registration workflow.</span></span> |
| <span data-ttu-id="bb300-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bb300-143">userPrincipalName</span></span> | <span data-ttu-id="bb300-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb300-144">String</span></span> | <span data-ttu-id="bb300-145">Nome principal do usuário que executa o fluxo de trabalho de redefinição ou registro.</span><span class="sxs-lookup"><span data-stu-id="bb300-145">User principal name of the user performing the reset or registration workflow.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bb300-146">Relações</span><span class="sxs-lookup"><span data-stu-id="bb300-146">Relationships</span></span>

<span data-ttu-id="bb300-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bb300-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb300-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb300-148">JSON representation</span></span>

<span data-ttu-id="bb300-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb300-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
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

